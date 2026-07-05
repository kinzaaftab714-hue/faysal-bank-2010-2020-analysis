# Contributing / Extending This Project

This project is structured so it can be extended by anyone (including future-you) without restructuring everything.

## Priority Extensions (Highest Impact First)

1. **Fill the financial data gap** — Add exact year-by-year figures (2010-2020) from Faysal Bank's annual reports into `09-data-and-charts/verified_data_points.csv`, then re-run `generate_charts.py`. This is the single highest-impact addition possible.
2. **Add peer bank data** — Extend the comparison in `07-comparative-analysis/` with exact deposit/profit figures for HBL, UBL, and Meezan Bank for the same years, enabling a real side-by-side chart instead of a qualitative comparison.
3. **Add primary source interviews** — If this project supports an academic submission, a short interview (even email Q&A) with a Faysal Bank branch manager or a banking industry analyst would elevate this from "desk research" to "primary research."

## Style Guidelines

- Keep claims cited — every factual statement should be traceable to `06-sources.md`
- Keep interpretation and fact clearly separated (see `08-critical-analysis/analysis.md` for the pattern)
- Prefer qualitative honesty over quantitative guessing — an acknowledged data gap is better than an invented number

## Setting Up Locally

```bash
git clone <your-repo-url>
cd faysal-bank-2010-2020
pip install -r 09-data-and-charts/requirements.txt
python 09-data-and-charts/generate_charts.py
```
