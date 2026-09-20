# NBA-Performance-and-Fan-Sentiment-Analytics
By: Navya Bhatia, Aakash Bhide, Vamsi Kolluri, and Sami Shikhare

Analyzed what drives NBA team popularity by combining team statistics, 62,388 unique tweets, and geographic data across 30 franchises. Built regression models to predict 2019–2020 win totals from historical results and evaluated how sentiment relates to success. Created interactive dashboards revealing fan engagement and overall performance trends.

# Project Objective
NBA team popularity is influenced by more than wins and losses. Successful teams often attract greater attention, but franchise history, star players, expectations, market size, and team narratives can also shape how fans react online.

This project examined the relationship between on-court performance, Twitter sentiment, and fan engagement during the 2019-2020 NBA season. It also evaluated whether historical team statistics could accurately predict season win totals and presented the findings through interactive Tableau dashboards.

# Objectives
- Compare team performance across all NBA franchises.
- Measure the relationship between winning and online fan sentiment.
- Evaluate fan engagement using tweet volume and retweet activity.
- Identify teams receiving more or less positive sentiment than expected.
- Predict 2019-2020 win totals using historical team statistics.
- Compare predicted wins with actual season results.
- Visualize geographic, performance, sentiment, and engagement patterns.

# Data
The project combines four datasets representing NBA performance, team geography, social media activity, and prediction results:

- nba_team_stats_00_to_23.csv - 716 team-season records with wins, losses, shooting, scoring, rebounding, assists, turnovers, and plus-minus statistics.
- teams.csv - location, arena, city, and franchise information for all 30 NBA teams.
- tableau_clean_start_scatter_lod.csv - team-level sentiment and engagement metrics created from 62,388 unique tweets.
- nba_prediction_results_tableau.csv - actual and predicted 2019-2020 win totals for all 30 teams.

The original Twitter data contained 116,825 records collected from approximately July through October 2020. After duplicate tweet IDs were removed, 62,388 unique tweets remained for analysis.

# Technologies Used
- Tableau
- Python
- R
- pandas
- Regression Modeling
- Sentiment Analysis
- Data cleaning and aggregation
- Data visualization
- Storytelling

# Repository Structure 
NBA-Performance-and-Fan-Sentiment-Analytics/
├── README.md
├── Final Graphs + Dashboard1 + Dashboard2.twbx
├── ISBA 2412 Final Project Plan.pdf
└── data/
    ├── nba_team_stats_00_to_23.csv
    ├── teams.csv
    ├── tableau_clean_start_scatter_lod.csv
    └── nba_prediction_results_tableau.csv

# Key Variables for Team Performance + Fan Sentiment and Engagement
Team Performance:
- Wins and Losses
- Win Percentage
- Points Scored
- Assists and Rebounds
- Field-goal Percentage
- Three-point Percentage
- Turnovers

Fan Sentiment and Engagement:
- Average and median sentiment scores
- Positive, neutral, and negative tweet shares
- Tweet count
- Total retweets
- Average author follower count
- Sentiment compared with the league average
- Engagement compared with market and league averages

# Analytical Workflow
1. Combined historical NBA performance, team-location, Twitter sentiment, and prediction data.
2. Removed duplicate tweet IDs, reducing 116,825 raw records to 62,388 unique tweets.
3. Aggregated sentiment, tweet volume, retweets, and audience metrics by team.
4. Calculated league-average performance, sentiment, and engagement benchmarks.
5. Compared 2019-2020 team wins and win percentages across all franchises.
6. Evaluated the relationship between team success and average Twitter sentiment.
7. Trained a regression model on team statistics from 2009-2010 through 2018-2019.
8. Predicted regular-season wins for all 30 teams in 2019-2020.
9. Compared predicted and actual wins using residuals and prediction-error categories.
10. Built 11 Tableau worksheets and two interactive dashboards to communicate the results.

# Dashboard Visualizations
1. NBA Franchise Location Map
2. Total Wins by Team
3. Win percentage compared with the League Average
4. Wins versus Average Fan Sentiment
5. Sentiment Interpretation and Residual Analysis
6. Actual versus Predicted Wins
7. Prediction-error Categories
8. Season Scoring compared with Performance
9. Three-point Percentage versus Wins

# Prediction Results
Teams Evaluated: 30
R-squared: 0.81
Mean Absolute Error (MAE): 4.15 Wins
Root Mean Squared Error: 5.11 Wins
Teams Predicted within 5 Wins: 21 of 30


The model demonstrated a strong relationship between predicted and actual wins. The most accurate prediction was for the Charlotte Hornets, with an error of only 0.06 wins. The Los Angeles Lakers and Oklahoma City Thunder were also predicted within one win of their actual results.

# Key Findings
- Winning alone did not fully explain fan sentiment or online engagement.
- Los Angeles Lakers and Toronto Raptors combined strong performance with highly positive sentiment.
- Milwaukee Bucks and Los Angeles Clippers achieved high win totals but received lower sentiment than several other successful teams.
- Orlando Magic generated strong positive sentiment despite fewer wins than top-ranked teams.
- Miami Heat recorded the highest tweet volume, showing that engagement does not always reflect positive sentiment.
- Historical statistics provided a strong foundation for predicting season win totals.
- Prediction errors increased for teams affected by injuries, roster changes, and disruptions during 2020.
- Higher scoring generally aligned with stronger performance, while defense, efficiency, and team balance also influenced success.

# Recommendations
- NBA teams should evaluate fan sentiment and engagement alongside performance. Winning alone does not fully explain fan behavior because team identity, star players, expectations, and market size also influence reactions.
- Teams should compare actual sentiment with expected sentiment and track tweet volume separately, since high engagement does not always indicate fan satisfaction.
- Historical statistics provide a useful forecasting baseline, but adding injuries, roster changes, player availability, and schedule difficulty could improve accuracy.
