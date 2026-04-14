# All-or-None Network Growth Model

Code accompanying *Densification and structural transitions in the
all-or-none copying model*.

## Files

- `all_or_none_model_code.ipynb` — main notebook reproducing all paper
  figures and the supplementary spectral-radius analysis.
- `cache/` — pre-computed simulation outputs as `.npz` files.
  Keep this folder in the same directory as the notebook to skip
  re-running the simulations.

## Usage

Open the notebook in Jupyter (or any compatible IDE) and run all cells.

- The first cell defines `MODE = "fast"` or `MODE = "paper"`:
  - `fast` — smaller `N`, fewer realisations, for quick checks.
  - `paper` — the configuration used for the figures in the paper.
- With the provided `cache/` folder, every cell returns instantly.
  Delete `cache/` to recompute from scratch.

## Structure

| Section | Content | Paper counterpart |
|---|---|---|
| 2 | Expected number of links                     | Fig. 2 |
| 3 | Fluctuations and self-averaging              | supplementary |
| 4 | Degree distribution (CCDF)                   | Fig. 3 |
| 5 | Triangles and clique hierarchy               | supplementary |
| 6 | Clustering and average shortest-path distance | Figs. 4 and 5 |
| 7 | Degree assortativity                         | Fig. 6 |
| 8 | Phase diagram                                | summary of Fig. 1 |
| 9 | Spectral radius (bonus)                      | supplementary |

## Requirements

- Python 3.9+
- `numpy`, `scipy`, `matplotlib`, `networkx`
