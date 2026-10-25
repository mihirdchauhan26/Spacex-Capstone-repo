# Winning Space Race with Data Science (IBM Data Science Capstone)

Predicting whether a SpaceX Falcon 9 first stage will land, to estimate launch cost and support a competing bid.

## Contents
| Path | Description |
|---|---|
| `notebooks/01_data_collection_api.ipynb` | SpaceX REST API data collection |
| `notebooks/02_data_collection_webscraping.ipynb` | Wikipedia web scraping (BeautifulSoup) |
| `notebooks/03_data_wrangling.ipynb` | Creating the `Class` landing label |
| `notebooks/04_eda_sql.ipynb` | EDA with SQL |
| `notebooks/05_eda_dataviz.ipynb` | EDA with Matplotlib / Seaborn |
| `notebooks/06_interactive_map_folium.ipynb` | Folium launch-site map |
| `notebooks/07_predictive_analysis.ipynb` | Classification models (LR, SVM, Tree, KNN) |
| `src/spacex_dash_app.py` | Plotly Dash dashboard |
| `SpaceX_Capstone_Presentation.pdf` | Final presentation |
| `images/`, `data/` | Screenshots and generated CSVs |

## Run
```bash
pip install -r requirements.txt
jupyter notebook          # run notebooks 01-07 in order
python src/spacex_dash_app.py
```

## Key findings
- Landing success rose from 0% (2010-2013) to about 80%+ in recent years.
- KSC LC-39A has the best success ratio; GTO is the hardest orbit.
- All four classifiers reach about 83% test accuracy; Decision Tree has the best CV score.
