## Filter-Bubble-ABM — Extended NetLogo Model, Experiments & Visuals

This repository contains everything needed to **replicate and extend** the study reported in our term-paper *“Filter Bubbles ABM model extension.”*
We rebuilt the triple-filter-bubble agent-based model (Geschke, Lorenz & Holtz, 2019) in NetLogo, added quantitative bubble-detection routines, ran a full parameter sweep, and visualised the results in R.

### Contents

| Path                                      | What it is                                                                                                                           |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| `model/TripleFilterBubble_Extended.nlogo` | **NetLogo model** with our extensions (bubble counter, tightness reporter, auto-stop).                                               |
| `experiments/bubble_grid_results.csv`     | **Raw output** from 288 simulations – one row per (latitude D, sharpness δ, seed) with bubble-count, tightness, etc.                 |
| `analysis/analysis_figures.R`             | **R script** (RStudio-ready) that ingests the CSV and reproduces all heat-maps, decision trees, and scatter plots used in the paper. |
| `figures/`                                | Pre-rendered PNGs of the key visuals for quick browsing.                                                                             |
| `docs/`                                   | The term-paper PDF and supplementary notes.                                                                                          |


### Why this matters

* **Model extension** adds concrete metrics (bubble count, σ-based tightness) so researchers can *measure* echo-chamber formation instead of eyeballing plots.
* **Open data & code** let anyone tweak parameters, re-run the grid, or bolt on new features (e.g., algorithmic filters).
* **Ready-made visuals** make it easy to drop the heat-maps and decision tree into slides, papers, or blog posts.

