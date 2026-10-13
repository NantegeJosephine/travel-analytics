# Safari & Travel Bookings Analytics

End-to-end analytics on safari/travel booking records (2023–2025): cleaning and exploring the raw bookings data with Python, then presenting it as an interactive Power BI dashboard (Safari Connect).

## What this project does

- **Cleans** three years of raw booking exports (deduplication, type fixes, consistency checks)
- **Analyzes** booking patterns across years — volume, pricing, and trends
- **Presents** the results in a Power BI dashboard for non-technical stakeholders

## Stack

| Layer | Tool |
| --- | --- |
| Environment | [uv](https://docs.astral.sh/uv/) (Python 3.12) |
| Analysis | Python, pandas, Jupyter |
| Visualization | Power BI Desktop |

## Repository structure

```
travel_project/
├── data/
│   ├── raw/          # source exports (not committed)
│   └── processed/    # cleaned outputs (not committed)
├── notebooks/        # cleaning + analysis notebooks
├── src/travel_project/
├── outputs/          # generated artifacts (not committed)
├── pyproject.toml
└── uv.lock
```

## Running it

```bash
uv sync          # create the environment from the lockfile
uv run jupyter lab
```

Then open the notebooks under `notebooks/` in order.

## Data

The booking and sales datasets used here are practice/course data and are **not committed** to this repository. Place your own exports under `data/raw/` to reproduce the analysis.

## Related

This project is featured as a case study on [Josephine Nantege's portfolio](https://github.com/NantegeJosephine). The companion Power BI dashboard (`Safari Connect`) is referenced there with screenshots.
