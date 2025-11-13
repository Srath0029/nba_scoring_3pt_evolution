🏀 NBA Scoring & 3-Point Evolution (1950–2024)

A data-driven exploration of how NBA scoring, shot selection, and 3-point usage have evolved across 70+ years — from the early eras of post play to today’s pace-and-space analytics revolution.
This project uses Python, pandas, matplotlib, and simple regression models to uncover long-term trends and project where the game is heading.

📁 Project Structure
nba_scoring_3pt_evolution/
│
├── NBA_Evolution_Notebook.ipynb     # Full analysis notebook
├── streamlit_app.py                 # Interactive dashboard
├── README.md                        # This file
└── (ignored) agg_by_year.csv        # Generated data

📊 Overview
<img width="400" height="1000" alt="image" src="https://github.com/user-attachments/assets/ad924c3f-a535-4fe9-a039-4e3afa0c2fbe" /> <img width="400" height="1000" alt="image" src="https://github.com/user-attachments/assets/342fbfac-c50b-4454-b525-b3b67119bbe1" />


<img width="400" height="1000" alt="image" src="https://github.com/user-attachments/assets/31525798-08bc-410b-ac8f-f6a0eb4d7fd6" />          <img width="400" height="1000" alt="image" src="https://github.com/user-attachments/assets/b00d30f0-7daa-4d6f-b3f1-4c7607c2c4a1" />



This project analyzes:

How average points per game (PPG) changed from 1950 to 2024

How 3-point attempts (3PA) and 3-point percentage (3P%) evolved over time

The impact of the 3-point line introduction in 1979

Trends that reveal where NBA offense is heading

Simple projections for future seasons based on recent statistical patterns

This analysis is ideal for:

Data science portfolio demonstration

Sports analytics case studies

Understanding macro-level NBA offensive trends

📦 Dataset

Source:
📚 NBA Player Stats 1950–2024 — Kaggle dataset by drgilermo
https://www.kaggle.com/datasets/drgilermo/nba-players-stats

Fields used:

Year

Games played (G)

Points (PTS)

3-Point Attempts (FG3A)

3-Point Makes (FG3M)

3-Point Percentage (FG3_PCT)

From these we compute:

Points per game (PPG)

3PA per game

3PM per game

🔍 Methodology
1. Data Cleaning

Standardized column names (PTS, FG3A, FG3M, etc.)

Converted season labels to integer years

Calculated per-game statistics

Handled missing pre-1979 3PT stats (set to 0 for volume, left % as NaN)

2. Aggregation

We aggregated all player stats by season (mean per-player metrics for each year).

3. Visualization

Using matplotlib, we plotted:

Average points per game (1950–2024)

Average 3PA per game

Average 3PM per game

Average 3P%

Correlation between 3PA and PPG

Simple projections for the next 5 years

4. Modeling

We applied simple linear regression on:

Recent 15-year 3PA trends

Recent 15-year scoring trends

To project:

Future league-wide PPG

Future 3PA per game

📈 Key Visualizations
📌 Evolution of Points per Game

Shows how scoring dipped in the early 2000s (slow pace, physical defense) before exploding again in the analytics era.

📌 Evolution of 3PA & 3PM per Game

Reveals the massive rise in 3-point volume since ~2012.

📌 3P% over Time

Stabilizes around modern values (~35–37%), even as volume skyrockets.

📌 Correlation — 3PA vs PPG

A positive relationship: as teams shoot more 3s, league scoring increases.

📌 Projection Plots

Simple regression suggests:

3PA/game will continue rising

PPG will likely increase modestly

🌟 Key Insights

3PT usage exploded in the 2010s, fundamentally changing offensive strategy.

Average 3PA per player per game increased by hundreds of percent since the early 1980s.

Despite the volume increase, 3P% remained stable, proving efficiency did not decline.

Scoring increases align strongly with increased pace and 3-point volume.

By projecting trends, the modern NBA will likely continue emphasizing:

Spacing

Perimeter-oriented offense

High-efficiency shot profiles

🚀 Future Improvements

Build more sophisticated time-series models (ARIMA, Prophet)

Integrate team-level metrics (pace, offensive rating)

Compare eras by normalizing pace and possessions

Add player-level clustering to identify shooter archetypes

Expand the Streamlit dashboard with filters and interactive charts

🖥️ Running the Notebook

Ensure you have Python 3.10+ and install dependencies:

pip install pandas numpy matplotlib scikit-learn ipykernel


Then open the notebook:

jupyter notebook NBA_Evolution_Notebook.ipynb

🖥️ Running the Streamlit App
pip install streamlit
streamlit run streamlit_app.py


Upload the generated agg_by_year.csv when prompted.

🏆 Final Notes

This project demonstrates:

Real-world data cleaning, EDA, and trend modeling

Ability to work with large sports datasets

Use of modern Python tools for visualization and projection

Clear communication of insights and data storytelling

Ideal for a data science, analytics, or sports-tech portfolio.
