# Steam Data Cleaning and Exploration

This project explores Steam game, review, and user-inventory data. The notebook covers data loading, schema and missing-value inspection, game-data cleaning, duplicate checks, and visual summaries.

## Project Files

- `steam_cleaning.ipynb` - analysis and visualizations.
- `dataset/steam_games.json.gz` - Steam game metadata.
- `dataset/australian_user_reviews.json.gz` - user reviews.
- `dataset/australian_users_items.json.gz` - games listed in user inventories.

The notebook reads the compressed JSON files directly from `dataset/`; they do not need to be extracted.

## Notebook Workflow

- Inspect the three raw datasets and compare their schemas.
- Measure missing values and review columns with substantial missingness.
- Clean game sentiment and prices, fill missing publisher and developer names, and remove selected columns and incomplete rows.
- Check duplicate identifiers and inspect examples from the datasets.
- Plot the most common game tags and the most frequently listed games in user inventories.

## Run

Use Python 3 from the repository root so the relative `dataset/` path resolves. Install the notebook dependencies:

```bash
python -m pip install pandas matplotlib notebook
```

Then open and run the notebook:

```bash
jupyter notebook steam_cleaning.ipynb
```