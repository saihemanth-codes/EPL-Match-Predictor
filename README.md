# Premier League Match Predictor

## Table of Contents
- [Project Overview](#project-overview)
- [Project Aim](#project-aim)
- [Libraries Used](#libraries-used)
- [Code Structure](#code-structure)
- [Data](#data)
- [Key Findings and Observations](#key-findings-and-observations)
- [Future Improvements](#future-improvements)


## Project Overview
This project implements a machine learning model to predict English Premier League match outcomes. The predictor uses historical match data, team statistics, and rolling averages to forecast match results, focusing on identifying winning probabilities. The model employs Random Forest Classification to capture complex patterns in football match dynamics.

## Project Aim
The primary objectives of this project are:
* Develop a reliable prediction model for Premier League match outcomes
* Utilize rolling averages of team performance metrics for improved accuracy
* Account for various factors including venue, timing, and historical performance
* Provide actionable insights for match result predictions

## Libraries Used
The project relies on the following Python libraries:
* `pandas`: Data manipulation and analysis
* `scikit-learn`: Machine learning implementation (RandomForestClassifier)
* Custom utilities for data preprocessing and feature engineering

## Code Structure
The main predictor code can be found in [`predictor.ipynb`](./predictor.ipynb). 

## Data
The dataset can be downloaded from [`matches.csv`](./data/matches.csv) here.

The dataset includes:
* Match dates and venues
* Team and opponent information
* Match statistics (goals, shots, possession, etc.)
* Final match results

The data preprocessing pipeline includes:
1. Date and time formatting
2. Categorical encoding of venues and teams
3. Generation of rolling averages for key statistics
4. Feature engineering for improved prediction accuracy

## Key Findings and Observations
The implemented Random Forest model shows promising results in predicting match outcomes. Key observations include:
* The model achieves approximately 66% accuracy (29/44) in predicting decisive matches
* Rolling averages of team performance metrics significantly improve prediction accuracy
* Venue and timing factors play important roles in match outcomes
* The model performs better when predicting matches for teams with consistent performance patterns

## Future Improvements
Potential enhancements for the project include:
* Integration of player-specific statistics
* Consideration of team formation and tactics
* Implementation of more sophisticated feature engineering
* Real-time data updates and predictions
