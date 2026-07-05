# Faysal Bank Limited — A Decade of Transformation (2010–2020)

![Faysal Bank Organizational Structure](./02-departments/org_chart.png)

## About This Project

This repository is an independent research and documentation project covering **Faysal Bank Limited (FBL)**, one of Pakistan's leading banks, focused on the ten-year period from **2010 to 2020**. It combines organizational research, real audited financial data, and a critical strategic analysis to answer one central question:

> *Was Faysal Bank's decade-long pivot — from a mid-sized conventional bank rebuilding after a major acquisition, to a bank committed to full Islamic conversion — a sound strategic response to its competitive position, and what were the trade-offs?*

Unlike a typical company profile, this project is built around **verified, audited financial data extracted directly from Faysal Bank's own annual report PDFs** (not estimates, not Wikipedia summaries), cross-validated across multiple reports, and benchmarked against Meezan Bank — Pakistan's largest Islamic bank — using real comparative figures.

> **Disclaimer:** This is an unofficial, independently compiled educational/research project. It is not affiliated with, endorsed by, or sponsored by Faysal Bank Limited, Meezan Bank, or any other institution mentioned. All information has been gathered from publicly available sources and should be verified against official communications for any formal, academic, or investment use. See [`06-sources.md`](./06-sources.md) for full references.

## What Makes This Project Different

Most student or portfolio projects on a company stop at description: history, departments, products. This one goes further by:

1. **Using primary-source financial data** — fetched directly from Faysal Bank's and Meezan Bank's own annual report PDFs, not secondary aggregators
2. **Cross-validating figures** across multiple overlapping annual reports to catch inconsistencies (and documenting the one known inconsistency — EPS restatement for bonus shares — rather than hiding it)
3. **Calculating real growth metrics (CAGR)** instead of just describing "the bank grew"
4. **Benchmarking against a named competitor** with the competitor's own real numbers, not a generic industry statement
5. **Stating a specific research question** and giving a balanced, evidence-based verdict — including what the data does *not* prove
6. **Disclosing every data gap honestly**, with the exact source document and page needed to close it — rather than filling gaps with invented numbers

## Table of Contents

| # | Section | What's Inside |
|---|---|---|
| 00 | [Executive Summary](./00-executive-summary.md) | One-page overview: the whole project in 2 minutes, for reviewers/recruiters short on time |
| 01 | [History & Timeline](./01-history-timeline/timeline.md) | Year-by-year milestones 2010–2020: the RBS acquisition, Islamic conversion announcement, branch expansion, and the 2020 SBP fine |
| 02 | [Departments](./02-departments/departments.md) | Full organizational breakdown — business lines, support functions, governance — with a visual org chart |
| 03 | [Functions & Services](./03-functions-services/services.md) | Core banking products and services, and how they shifted from conventional to Islamic banking |
| 04 | [Financial Overview](./04-financial-overview/overview.md) | Real audited figures 2011–2018 & 2020: deposits, assets, profit, EPS, equity, ROE/ROA — with charts and CAGR analysis |
| 05 | [Digital Transformation](./05-digital-transformation/digital.md) | IT/core-banking modernization during the decade, and what it set up for post-2020 digital products |
| 06 | [Sources](./06-sources.md) | Every source used, including direct links to all 11 annual report PDFs (2010–2020) |
| 07 | [Comparative Analysis](./07-comparative-analysis/peer-comparison.md) | Faysal Bank vs. Meezan Bank, 2011–2018 — real audited-data comparison with CAGR charts and a genuinely non-obvious finding |
| 08 | [Critical Analysis](./08-critical-analysis/analysis.md) | The stated research question, what worked, what's debatable, and a balanced final verdict |
| 09 | [Data & Charts](./09-data-and-charts/README.md) | The raw CSV dataset, the Python script that generates every chart, and full data-provenance notes |

## Key Findings at a Glance

| Metric | Faysal Bank (2011–2018 CAGR) | Meezan Bank (2011–2018 CAGR) |
|---|---|---|
| Deposits | 9.7% | 24.5% |
| Total Assets | 10.8% | 24.4% |
| **Profit After Tax** | **20.9%** | 14.9% |
| Branch Network | 8.5% | 13.3% |

Meezan Bank scaled up faster; Faysal Bank converted its (smaller) growth into profit faster. See [07-comparative-analysis](./07-comparative-analysis/peer-comparison.md) for the full reasoning behind this finding.

## Why 2010–2020?

This decade marks one of the most transformative periods in Faysal Bank's history:
- **2010**: Acquisition of RBS Pakistan's operations (~£34 million), significantly expanding the branch network overnight
- **2011–2013**: Post-acquisition integration, workforce rationalization, and a near-flat profit period
- **2014**: Public announcement of a full conversion to Islamic banking within 3–5 years
- **2015–2020**: Gradual branch conversion, accelerating profitability, and rapid network expansion — culminating in a fully Islamic-converted bank by 2023 (just after this project's window)

## Methodology

This project distinguishes clearly, throughout every section, between three types of content:
- **Verified facts** — cited to a specific source, usually a specific annual report and page (see [06-sources.md](./06-sources.md))
- **Reasonable strategic inference** — logical connections drawn from verified facts, explicitly labeled as interpretation rather than fact
- **Open questions** — areas where available public data is insufficient for a firm conclusion, flagged honestly rather than papered over with invented numbers

This approach is intentional: a research project that admits its data gaps and shows exactly how to close them is more credible — to a recruiter, a scholarship committee, or a general reader — than one that presents estimates as certainties.

## Repository Structure

```
faysal-bank-2010-2020/
├── 00-executive-summary.md
├── 01-history-timeline/
│   └── timeline.md
├── 02-departments/
│   ├── departments.md
│   └── org_chart.png
├── 03-functions-services/
│   └── services.md
├── 04-financial-overview/
│   └── overview.md
├── 05-digital-transformation/
│   └── digital.md
├── 06-sources.md
├── 07-comparative-analysis/
│   ├── peer-comparison.md
│   ├── peer_comparison_data.csv
│   ├── generate_comparison_charts.py
│   └── chart_*.png
├── 08-critical-analysis/
│   └── analysis.md
├── 09-data-and-charts/
│   ├── README.md
│   ├── verified_data_points.csv
│   ├── generate_charts.py
│   ├── requirements.txt
│   └── chart_*.png
├── CONTRIBUTING.md
├── LICENSE.md
├── .gitignore
└── README.md
```

## How to Use This Repo

- Each numbered folder is self-contained and can be read independently — start with `00-executive-summary.md` if you're short on time.
- All Markdown files are written to render cleanly on GitHub, with images and cross-links working out of the box.
- To regenerate any chart from the raw data: `pip install -r 09-data-and-charts/requirements.txt` then `python 09-data-and-charts/generate_charts.py` (or the equivalent script in `07-comparative-analysis/`).
- See [CONTRIBUTING.md](./CONTRIBUTING.md) for the highest-impact ways to extend this project further (closing the 2010/2019 data gaps, adding more peer banks, etc.).

## License

See [LICENSE.md](./LICENSE.md). This documentation is provided for educational purposes. All trademarks, logos, and brand names belong to their respective owners (Faysal Bank Limited, Meezan Bank).
