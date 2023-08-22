# Project 4: ML Predictions on NBA Salaries

## Overview
Through compiling the statistics of players in the NBA, we aim to predict the potential salary a player will make in the future using machine learning algorithms.

## Directory
- `Resources` contains all relevant .CSV files used for analysis
- `Scripts` contains all relevant code files used to run the analysis

## ETL Process
1. Data Collection: Collect historical NBA player data, including player statistics, draft position, team performance, salary information, player attributes, and any other relevant features that could influence contract decisions.
2. Data Preprocessing: Clean the data by handling missing values, outliers, and inconsistencies. Normalize or scale numerical features and encode categorical features using techniques like one-hot encoding or label encoding.
3. Feature Engineering: Create meaningful features that could impact a player's contract, such as player performance metrics (e.g., points per game, rebounds, assists), team performance (e.g., wins, playoffs), player rankings, draft position, All-Star selections, and any other relevant attributes.
4. Model Selection: Choose appropriate machine learning algorithms for regression, as predicting contract values is a regression problem. You can consider algorithms like Linear Regression, Random Forest, Gradient Boosting, or even more advanced models like Neural Networks.
5. Model Training: Train the selected model using the training dataset. Adjust hyperparameters as needed and utilize techniques like cross-validation to ensure robustness.
6. Model Evaluation: Evaluate the model's performance using the testing dataset. Common regression metrics include Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE). Additionally, you could analyze feature importance to understand which factors contribute most to contract predictions.


## Data Model Implementation
We created a model based on some of the following (but not limited to) the following criteria: Points, Blocks, Rebounds, Assists, and historical salary information. We found data from several different sources and combined them to run our model on.

Using a linear regression model which was trained using SDG regressor (Stochastic Gradient Descent)

We tried to build out a more comprehensive dataset to improve the foundation of our model. While more data meant more information to use, it also meant more pre-processing and nuance to address.
## Data Model Optimization
To optimize, the following changes really impacted the model's performance
- Pre-processing
    - Properly encoding categorical data
    - Not Scaling Categorical data
- Tuning
    - Moving from StandardScaler to MinMaxScaler
    - Raising the learning rate
    - Removing regularization
- Started testing on the 2018-2019 salary data and moved year by year with varying (ultimately increasing) model performance

You can find the data model evaluation process showing iterative changes the resulting model performance within the script itself.

## Visualizations


![](/images/KALSDFSLKFJ)

## Contributors
- Matthew Reyes `mattbreyes`
- Ryan Kincheloe `TonysTinyToes`
- Emma Ng `sumiemma`
- Stelios Kosmidis `SteliosKosmidis`
- Harman Malhi `hmalhi85`
- Akhyar Zaman `akzaman47`