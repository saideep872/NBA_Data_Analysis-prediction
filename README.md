# NBA Playoff Performance Data Science Project - README

## Overview
This project analyzes the National Basketball Association (NBA) playoff and regular season data from 2014 to 2023, focusing on team and player statistics to answer key questions about game performance, playoff progression, and predict future outcomes. The analysis aims to provide insights into the factors that influence game wins, playoff outcomes, and key player performance metrics.

## Structure of the Project
The project is divided into three main parts:

### Part 1: Data Cleaning and Exploratory Analysis
In this section, the goal was to analyze historical NBA data at both the team and player levels to answer various questions. The questions revolved around effective field goal percentages (eFG%), offensive rebound influence on game wins, player availability, and other performance metrics. Key tasks in this section included:
- Filtering the dataset to focus on specific seasons, teams, or metrics.
- Calculating offensive and defensive metrics, such as eFG% and win percentages.
- Visualizing data trends, including effective shooting efficiency and home-court advantages.

### Part 2: Playoff Series Modeling
This part of the project involved creating a predictive model that forecasts the outcome of NBA playoff series. The model predicts the winner and the number of games in a playoff series based on historical data.
- The model leverages metrics like offensive rating (ORTG), defensive rating (DRTG), and net rating to assess team strengths.
- A Random Forest model was used for prediction due to its robustness in handling complex features and its interpretability.
- The model output includes the probability of each team winning the series and predicts the number of games in the series.
- Visualizations provide an overview of team chances for advancing in the playoffs, making the analysis useful for decision-makers.

### Part 3: Insights and Model Performance
In the final section, insights were drawn from the model results to understand team performances and highlight cases where the model's expectations were not met.
- Two teams that underperformed despite having strong metrics were identified: the Lakers and the Nuggets. One team's underperformance was attributed to bad luck, while the other was linked to limited data samples and a lack of hyperparameter tuning.
- The section also includes recommendations on improving the model by incorporating real-time coaching strategies, performing hyperparameter tuning, and further noise reduction techniques.

## Dataset Information
The project uses two datasets:
- **Player Game Data (`player_game_data.csv`)**: Contains player-level statistics for games from 2014 to 2023.
- **Team Game Data (`team_game_data.csv`)**: Contains team-level statistics, covering both regular season and playoff games.

These datasets include comprehensive game statistics, including field goals made, three-point attempts, offensive rebounds, win/loss outcomes, and other metrics.

## Dependencies and Setup
To replicate the project, the following software and packages are required:
- **R Programming Language**: Used for data analysis, modeling, and visualization.
- **Libraries**: The following R packages were used:
  - `dplyr`: For data manipulation.
  - `ggplot2`: For data visualization.
  - `caret`, `smotefamily`, `randomForest`: For model training, balancing data, and predictions.
  - `tidyverse`, `naniar`, `readr`: For various data processing and visualization tasks.

To run the analysis, ensure the R environment is properly set up with the above libraries installed.

## How to Run the Analysis
1. **Load the Datasets**: Make sure `player_game_data.csv` and `team_game_data.csv` are available in your working directory. Load these datasets using the appropriate `read_csv()` commands.
2. **Data Preprocessing**: Follow the steps in Part 1 to clean the data, filter relevant games, and compute required metrics.
3. **Model Training**: Use the script in Part 2 to train the Random Forest model on historical playoff data.
4. **Generate Predictions**: Apply the trained model to the test dataset to predict playoff series outcomes for the 2024 NBA playoffs.
5. **Visualize Insights**: Create visualizations as needed to present the results of the analysis.

## Results Summary
- The team with the higher effective field goal percentage (eFG%) wins approximately 81.6% of the time.
- The team with more offensive rebounds wins only about 46.2% of the time, suggesting that shooting efficiency has a greater impact on game outcomes than additional possession opportunities.
- Players who score at least 25 points per game and play 25% of their games are available for an average of 99.7% of their games.
- Home-court advantage plays a significant role, especially in the first round of the playoffs, where teams with home-court advantage won 83.3% of the time.

## Future Work
- **Model Improvements**: Implement hyperparameter tuning for the Random Forest model, incorporate more advanced features such as real-time coaching strategies, and improve the data quality by reducing noise.
- **Feature Engineering**: Extract more meaningful features from the data, such as player fatigue metrics, clutch performance, or injury data, which could enhance model accuracy.
- **Deeper Analysis**: Analyze individual player impacts on a game-by-game basis to understand which players are most critical to playoff success.

## Contact Information
For any questions or further discussion, please feel free to reach out to Saideep Reddy Thaduru.

Thank you for your interest in this NBA Playoff Performance Data Science Project!

