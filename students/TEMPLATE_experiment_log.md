# Experiment Log (Your Name)

For each experiment you run this semester:
1. Copy the template block below.
2. Fill it in.
3. Add it to the bottom of this file.

---

## Experiment Template

### Run #: 
### Date:
### Goal / Question:
(What are you testing or curious about?)

### Setup:
(What data, model, hyperparameters, preprocessing did you use?)

### Results:
(Key metrics: accuracy, precision/recall, confusion matrix, etc.)

### Reflection:
(What worked? What didn’t? What would you try next?)


# Example Experiment Log — Taiwo 

## Run 1 — 2025-09-04
- **Goal / Question**: What happens if I change `n_estimators` from 100 to 200?
- **Setup**: Baseline Random Forest, train/test split = 80/20
- **Results**: Accuracy = 0.84, Precision = 0.72, Recall = 0.66
- **Reflection**: Increasing estimators gave a small accuracy bump. Took longer to train. Worth it? Maybe.

---

## Run 2 — 2025-09-06
- **Goal / Question**: Compare Random Forest vs Logistic Regression
- **Setup**: Same preprocessing as before
- **Results**: RF Acc = 0.85, LogReg Acc = 0.79
- **Reflection**: LogReg underfit the data. Nice reminder that not all models capture interactions.





Experiment - Alok
Run: 1 
Date: 2025-09-08
Goal / Question:
Determine whether GridSearchCV or RandomizedSearchCV is faster
Setup:
Create a GridSearchCV and RandomizedSearchCV parameter grid, then time each one’s search time and print it out
Results:
Grid - 89.34 seconds
Randomized - 127.02 seconds
Reflection:
Randomized spent more time searching. However, randomized search was used on a larger group of parameters and its number of iterations was greater than grid searches.


Run: 2
Date: 2025-09-08
Goal / Question:
Determine if there is a difference between the best parameters for GridSearchCV or RandomizedSearchCV
Setup:
Run a GridSearchCV and RandomizedSearchCV and print out each one’s optimal parameters
Results:
Grid - max_depth:20, n_estimators:100
Randomized - max_depth:20, min_samples_split:4, n_estimators:121
Reflection:
They had relatively similar estimators, Randomized just searching through more variation, had slightly more optimal parameters


Run: 3
Date: 2025-09-08
Goal / Question:
When would you choose GridSearchCV or RandomizedSearchCV in practice
Reflection:
In larger pools of parameters, GridSearchCV spends a lot of time, meaning the randomized search could be used for more optimal parameters. This can also reduce the risk of overfitting the model’s parameters.

