# Stolen Base Success Prediction Model
This project presents a predictive model designed to estimate the probability of a successful stolen base attempt, specifically when a runner tries to steal second base with no other runners on the field. The model leverages a variety of features related to the catcher, pitcher, runner, and game situation to make accurate predictions.

## Project Overview
**1. Objective:**
- Predict whether a stolen base attempt will be successful based on various contextual factors.

**2. Data Selection and Preparation:**
- Focused on attempts to steal second base with a runner on first.
- Excluded pickoff attempts and irrelevant plays like wild pitches.
-Handled missing data by imputation, particularly for metrics like Pop Time, exchange times, and historical success rates.

**3. Feature Engineering:**
- Catcher: Pop time, exchange time.
- Pitcher: Plate time, handedness, pitch type usage.
- Runner: Lead distance, secondary lead distance, sprint speed.
- Game Context: Inning, score, balls, strikes, outs, defensive team lead.
- Added historical stolen base success rates for pitchers, catchers, and runners.

**4. Modeling Approach:**
- Tested various classification models, including logistic regression and gradient-boosted trees.
- Evaluated models using the F1-score to balance between maximizing successful steals and minimizing caught steals.

**5. Results:**
- The final model, using logistic regression with all available features, achieved an F1-score of 0.861.
- Feature importance analysis highlighted secondary lead distance and historical success rates as key predictors.

**6. Visualization:**
- Created plots to visualize the relationship between features and the probability of a successful steal.
- Visualized model performance using confusion matrices and probability density plots.

## How to Use the Model
- The model can calculate the probability of a successful steal in a given game situation.
- By comparing the model's prediction with the break-even success rate, teams can decide whether a steal attempt is advisable.

## Future Work
- Consider expanding the model to include more complex game situations, such as multiple base runners and different counts.
- Investigate the impact of the 2023 MLB rule changes on the model’s predictions.
