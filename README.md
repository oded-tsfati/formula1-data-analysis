# Formula 1 – Exploratory Data Analysis (1950 → today)

Exploratory analysis of the complete Formula 1 World Championship history with **pandas**, **Matplotlib** and **Seaborn**.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/oded-tsfati/Formula1/blob/main/Formula1.ipynb)

## Questions explored
- **Who wins the most?** Top 10 drivers and top 10 constructors by race wins
- **Driver vs. constructor** – which teams each top driver won with
- **Season view** – race winners for any chosen year (function `get_year_winners(year)`)
- **How big is the grid?** Number of drivers and constructors per season since 1950
- **Does qualifying matter?** Starting grid position vs. finishing position, with regression line – for all circuits and for the Monaco Grand Prix since 2010
- **Race story** – lap-by-lap position chart for every driver in a selected race, plus lap-time chart per driver

## Data
[Formula 1 World Championship (1950 – 2023)](https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020) on Kaggle (Ergast data): `drivers`, `results`, `races`, `constructors`, `constructor_results`, `lap_times` CSV files. Data files are not included in this repository – download them from Kaggle.

## Techniques
Merging several related tables (relational joins in pandas) · group-by aggregations · reusable analysis functions · regression plots · time-delta parsing of lap times · multi-line plots

## Tech stack
Python · pandas · NumPy · Matplotlib · Seaborn · Google Colab

## How to run
```bash
pip install -r requirements.txt
jupyter notebook Formula1.ipynb
```
Adjust the CSV paths in the "loading CSV files" cell (originally `/content/drive/MyDrive/Formula1/...`) to where you saved the Kaggle files.
