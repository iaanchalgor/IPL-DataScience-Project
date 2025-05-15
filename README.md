# IPL-DataScience-Project

# IPL Match Winner Prediction

 Project Overview

This project aims to predict the winner of Indian Premier League (IPL) cricket matches using historical data. We use two datasets:

- **Matches dataset**: Contains details about each match (teams, venue, toss winner, season, etc.).
- **Deliveries dataset**: Ball-by-ball data of each match including runs, wickets, players involved, etc.

The goal is to build a machine learning model that predicts the match winner based on factors like teams playing, toss winner, venue, and season.



Data Understanding

- Matches dataset columns**:  
  `id`, `season`, `city`, `date`, `match_type`, `player_of_match`, `venue`, `team1`, `team2`, `toss_winner`, `toss_decision`, `winner`, `result`, `result_margin`, `target_runs`, `target_overs`, `super_over`, `method`, `umpire1`, `umpire2`

- Deliveries dataset columns**:  
  `match_id`, `inning`, `batting_team`, `bowling_team`, `over`, `ball`, `batter`, `bowler`, `non_striker`, `batsman_runs`, `extra_runs`, `total_runs`, `extras_type`, `is_wicket`, `player_dismissed`, `dismissal_kind`, `fielder`



Steps Taken

1. Data Loading  
   Loaded both datasets using Pandas and explored basic structure and columns.

2. Exploratory Data Analysis (EDA)  
   - Examined top batsmen, bowlers, and teams by runs and wickets.  
   - Visualized season-wise runs scored by teams.  
   - Checked dismissal types and player performances.

3. Feature Selection
   Selected important features for prediction:  
   `team1`, `team2`, `toss_winner`, `toss_decision`, `venue`, `city`, `season`.

4. Data Preprocessing  
   - Handled categorical variables using label encoding.  
   - Split data into training and testing sets.

5. Modeling  
   - Built a Random Forest Classifier model to predict the winner.  
   - Evaluated model accuracy (~54%).

6. Future Improvements  
   - Improve accuracy by tuning hyperparameters.  
   - Experiment with more advanced algorithms like XGBoost, LightGBM.  
   - Incorporate player-level data and recent form.  
   - Build a web app for interactive predictions.



Dependencies
pandas
numpy
scikit-learn
matplotlib
seaborn

Author
Aanchal Gor
MSc in AI/ML Student
Email: aanchalgor9@gmail.com
