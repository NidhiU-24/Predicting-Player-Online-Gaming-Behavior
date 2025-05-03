# Predicting Player Online Gaming Behavior
The project focused on predicting player engagement in online gaming, specifically identifying "high-engagement" players using behavioral, demographic, and game-specific data from a Steam-based dataset.

Problem Definition: Understanding that player retention is key to sustainable business; goal was to predict high engagement and understand purchase behaviors.

## Data Exploration:

1. Dataset had 13 features related to demographics, gameplay, and engagement.
2. Observed a class imbalance (only ~26% were high-engagement players).
3. Variables like SessionsPerWeek and AvgSessionDurationMinutes were found to be strong predictors of engagement.

## Preprocessing:

1. One-hot encoding used for categorical features.
2. No missing values found.
3. Target variable redefined into a binary classification (High vs. Low-Medium engagement).

## Model Development:

1. Four models were tested: Logistic Regression, Random Forest, K-Nearest Neighbors (KNN), and Multi-Layer Perceptron (MLP).
2. Hyperparameter tuning was performed for each model to improve performance.
3. SHAP analysis was used to interpret feature importance.

## Model Performance:

1. Random Forest was the best model with highest accuracy (~95% after tuning).
2. Key predictors across models were SessionsPerWeek, AvgSessionDurationMinutes, and AchievementsUnlocked.
3. KNN performed the worst compared to others, while MLP was a close second to Random Forest.

## Key Business Insights:

1. Session frequency and duration are the most important for retention.
2. Regional differences matter for marketing strategies.
3. Adjustable game difficulty improves engagement.
4. Strong recommendation to use ensemble models like Random Forest for retention prediction.

## Limitations and Future Directions:

1. The study used cross-sectional data (no time-series evolution).
2. No causal inferences could be made.
3. Future work could involve time-series analysis, social network analysis, and churn prediction models.
