# IPL Analytics Dashboard

An end-to-end IPL analytics project combining **Python, Power BI, and Machine Learning** to analyze match outcomes, player performance, team performance, and venue trends across IPL seasons from 2008–2019.

## Project Overview

This project explores IPL match data to identify meaningful insights across:

- Match and season performance
- Team win percentages
- Player batting performance
- Player bowling performance
- Venue-level statistics
- Toss decisions and match outcomes
- Match scoring trends

The project also includes a **machine learning model for predicting match winners**.

## Tools & Technologies

- **Python** — Data cleaning, analysis, feature engineering and machine learning
- **Pandas & NumPy** — Data manipulation and analysis
- **Scikit-learn** — Model evaluation and preprocessing
- **XGBoost** — Match winner prediction
- **Power BI** — Interactive dashboard and data visualization
- **Excel / CSV** — Source and processed datasets

## Power BI Dashboard

The dashboard provides an overview of IPL performance through:

- Total Matches
- Highest Match Total
- Average Runs per Match
- Toss Win & Match Win percentage
- Average Runs by Season
- Top 10 Run Scorers
- Top 10 Wicket Takers
- Team Win Percentage
- Top 10 Venues by Matches
- Top 10 Venues by Average Runs
- Matches by IPL Season
- Toss Decision Analysis

## Machine Learning

Multiple classification models were evaluated for predicting match winners, including:

- Logistic Regression
- Random Forest
- XGBoost

### Final XGBoost Performance

| Metric | Score |
|---|---:|
| Accuracy | 67.80% |
| Precision | 60.00% |
| Recall | 52.17% |
| F1 Score | 55.81% |
| ROC-AUC | 68.60% |

XGBoost achieved the strongest overall performance among the evaluated models.

## Feature Importance

The XGBoost model identified several influential features, including:

- Venue
- Team combinations
- Historical win-rate difference
- Venue chasing win rate

This suggests that both **team history and venue-specific performance** contribute to predicting match outcomes.

## Repository Contents

| File | Description |
|---|---|
| `ipl.analysis.pbix` | Power BI dashboard |
| `matches_clean.csv` | Cleaned match-level dataset |
| `matches_powerbi.csv` | Dataset prepared for Power BI |
| `match_runs.csv` | Match-level run statistics |
| `player_batting.csv` | Aggregated batting statistics |
| `player_bowling.csv` | Aggregated bowling statistics |
| `players_clean.csv` | Cleaned player dataset |
| `team_stats.csv` | Team performance statistics |
| `venue_avg_runs.csv` | Venue-level average run statistics |
| `MATCHES.xlsx` | Original match data |
| `PLAYERS.xlsx` | Original player data |
| `DELIVERIES.xlsx` | Original ball-by-ball delivery data |

## Key Insights

- Chennai Super Kings and Mumbai Indians show consistently strong historical performance.
- V Kohli, SK Raina and RG Sharma are among the leading run scorers in the analyzed dataset.
- Venue characteristics have a measurable influence on match outcomes and scoring.
- Historical team performance and venue-related features contribute significantly to match winner prediction.

## Project Author

**Anushka V Mankar**
