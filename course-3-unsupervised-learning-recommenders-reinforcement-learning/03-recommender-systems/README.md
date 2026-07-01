# Recommender Systems: Collaborative Filtering & Content-Based Filtering

From-scratch NumPy implementation of two recommender system approaches,
following Andrew Ng's ML Specialization (Course 3, Week 2) — with full
math derivations, manually-derived gradients, gradient checking, and
honest observations on where each method holds up and where it breaks.

## What's in here

**Collaborative Filtering**
- Cost function and gradient derivation from first principles
- Vectorized implementation (cost, gradients, training loop)
- Numerical gradient checking (verified to ~1e-9 relative error)
- Cold-start failure demonstrated directly: a movie with zero ratings gets
  a mathematically frozen feature vector — not a tuning problem, a
  structural one (see Observations in the notebook)

**Content-Based Filtering**
- Two-tower neural network (user tower + movie tower → dot product)
- Forward and backward pass written by hand — including the gradient
  split at the dot product where a single loss flows into two separate
  networks
- A real bug found via gradient checking (a double-normalization issue
  in the backward pass — see the notebook for the full story) and fixed
- Demonstrated fix for item cold-start: a never-rated movie still gets a
  sensible prediction, because its embedding depends only on features,
  not rating history

**Comparison**
- Side-by-side breakdown of when to reach for each method, with actual
  RMSE numbers from this notebook's runs, not just theory

## Key results

| | Collaborative Filtering | Content-Based Filtering |
|---|---|---|
| RMSE (rated) | 0.39 | 0.27 |
| RMSE (unrated/held-out) | 1.84 | 2.42 |
| Handles new item, zero ratings | ❌ | ✅ |
| Needs feature metadata | ❌ | ✅ (required) |

## Notes on the data

All data is synthetic — generated from random "ground truth" embeddings,
then masked to simulate realistic ratings sparsity (~50-60% observed).
This is intentional: it makes it possible to check predictions against a
known ground truth on *unrated* entries, which you'd never have with real
data.

## Known gap

Mean normalization (the standard fix for **new-user** cold-start, as
opposed to the new-*item* cold-start demonstrated here) isn't implemented
in this version. What's shown instead is item-level cold-start via a
zero-rated row. Worth adding as a follow-up.

## Requirements

- Python 3.11+
- NumPy only — no ML frameworks used, by design