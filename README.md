# Tool Window Open Duration: Auto vs Manual

A study, analyzing some toolwindow usage data on a non-large dataset and determining whether there's a meaningful difference in how long the tool window stays open depending on how it was opened.

What’s inside
- main.ipynb — the primary notebook with the full analysis pipeline.
- requirements.txt — Python dependencies.
- PDF file, describing the whole pipeline.

## Quick start
- Use Python 3.12
- Open the project folder.
- Configure the interpreter to use .venv (or create a new one via the IDE).
- Install dependencies from requirements.txt.
- Open main.ipynb and execute the cells sequentially.

Expected outputs
- Printed results of statistical tests (KS, Mann–Whitney, binomial test), Cliff’s Delta estimate, and a 95% bootstrap confidence interval.
- Saved plots in the project root:
  - manual_vs_auto.png — distributions before/after outlier filtering.
  - manual_vs_auto_per_user.png — per‑user average durations (manual vs auto).
  - bootstrap_distribution.png — bootstrap distribution for Cliff’s Delta.

Notes
- Some Pandas and SmallSampleWarning messages are suppressed in the notebook for cleaner output.
