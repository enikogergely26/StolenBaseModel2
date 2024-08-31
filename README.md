# Stolen Base Success Prediction
This project aims to develop a predictive model to determine the probability of a successful stolen base attempt when a runner takes off for an empty second base. The model uses various features related to the runner, pitcher, and catcher to assess the likelihood of success and inform decision-making during games.

## Key Steps and Methodology
**1. Data Selection:** Focused on stolen base attempts to second base with only a runner on first. Excluded irrelevant data such as pickoff attempts and wild pitches.

**2. Feature Engineering:**
- Created features like lead distance, pitcher's arsenal, and historical stolen base success rates.
- Addressed missing data with imputation techniques and excluded outliers.
- Applied mean encoding to categorical variables like inning, score, and count.

**3. Visualization and Analysis:**
- Visualized key metrics using seaborn to identify important features for classification.
- Analyzed correlations to select the most predictive features, such as secondary lead distance and historical success rates.

**4. Modeling:**
- Tested various classifiers, optimizing for F1-score due to the imbalanced nature of the data.
- Evaluated feature importance and validated the model using double density plots and confusion matrices.

## Next Steps
- Feature Expansion: Incorporate additional features like hitter's plate discipline and pitch information.
- Broaden Scope: Extend the model to cover more complex game situations, including multiple base runners and pickoff events.
