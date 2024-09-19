# NBA Career Outcome Multiclassifier 

This project aims to predict the career outcomes of NBA players based on their individual in-game statistics. By leveraging various machine learning models, the project explores the relationship between player performance data and career success.

## Project Overview 
The goal is to train multiple machine learning models to correctly predict the career outcomes of NBA players. Each player was manually classified into one of five career outcome categories based on their highest career achievements. The project involves data cleaning, exploratory data analysis (EDA), model training, and evaluation.

## Data
The data used to train the models initially consisted of up to 20,000 observations but was trimmed down to 2,722 rows and can be found [here](https://www.kaggle.com/datasets/sumitrodatta/nba-aba-baa-stats?resource=download&select=Advanced.csv).

## Technologies Used
- Python
- Packages include:
    - Pandas
    - Numpy
    - Scikit-learn
    - Matplotlib/Seaborn/Altair
    
## Career Outcome Classes
Each player was classifed into one out of the following career outcome categories:
- Elite (Most valuable player/Defensive player of the year/All NBA 1st or 2nd team)
- All-Star
- Starter (Played at least 50 games or 2000 minutes a season)
- Roster Player
- Out of the league

## Exploratory Data Analysis (EDA)
General exploratory data analysis (EDA) was performed to identify potential problems with the data, including issues with normality, missing values, and correlation.

## Machine Learning Models Used
The following machine learning models were trained and evaluated:
- Logisitc Regression
- Random Forest
- Gradient Boosted Trees
- K-Nearest Neighbors (KNN)

## Model Training
- Stratified K-Fold Cross-Validation: Used to ensure the data used to train the models were split evenly across the five career outcome classes, to prevent imbalance issues. 

- Hyperparameter Tuning: Optimizes model performance by finding the best parameter values

## Evaluation Metrics
- Accuracy: Measures how often the models correctly classify a player into the right career outcome.
-ROC AUC (Receiver Operating Characteristic Area Under the Curve): Used to assess the ability of the models to distinguish between classes, particularly useful for imbalanced datasets.

## Results
After training and evaluating the models, the logisitic regression and gradient boosting models performed the best with both models having over 70% accuracy and ROC AUC scores above 0.9

## Future Improvements
- Feature Engineering: Investigate new features that could further improve model performance, such as advanced stats (team dynamics, player position, player playing style) and external factors (injuries, trades, etc.)

## Potential Real World Use Cases
This project has several potential real-world applications in sports analytics, particularly in basketball:

- Player Scouting: Teams can use the models to predict the future career trajectory of players based on early-career performance, helping make informed decisions in trades and free agency

- Performance Evaluation: Coaching staff can assess players' potential based on their in-game statistics, allowing them to optimize training programs and game strategies to enhance career outcomes.

- Contract Negotiations: Teams can use the predictions to guide contract discussions, offering higher-value contracts to players with a predicted higher career ceiling.

