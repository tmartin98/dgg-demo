# Diffusion Graph Generator: static demo

A read-only snapshot of the Diffusion Graph Generator web app, made on 2026-10-22. Open it at https://tmartin98.github.io/dgg-demo/.
No sign-in is necessary. The guided tour starts on the first visit. You cannot start a Job in this demo.

## Data and licence

The files in `snapshot/` come from the IBM Transactions for Anti Money Laundering (AML) data set
(E. Altman et al., "Realistic Synthetic Financial Transactions for Anti-Money Laundering Models", NeurIPS 2023,
Kaggle). The IBM data is a simulation, not real bank data. It is licensed under the Community Data License
Agreement - Sharing - Version 1.0 (`LICENSE-DATA`).

This snapshot is Enhanced Data under that licence, and it is published under the same licence with no further
restrictions. Our changes to the IBM data:

- We sampled Account graphs (Base, Holdout and Validation Graphs) from the IBM transfers.
- A diffusion model made Synthetic Graphs with new Accounts. Their transfers are copies of real Base Graph transfers.
- We injected copies of IBM laundering patterns (Smurfing, Drain Chain, Cycle) into the Synthetic Graphs.
- We added model scores, alert flags, SHAP values, aggregates and metrics.
- The files are JSON answers of the web app API, as of 2026-10-22.

The web app code in this repository (`index.html`, `404.html`, `assets/`) is not licensed for reuse.
