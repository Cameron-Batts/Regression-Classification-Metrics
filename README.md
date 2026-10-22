# Regression Interpretation and Classification Metrics
**Cameron Batts**

## Problem
Explain regression coefficients, calculate classification tradeoffs and fit a simple advertising-sales model.

## Approach
Interpret archived vehicle-price OLS and bank-deposit logistic model summaries, compute metrics for a supplied confusion matrix, and fit sales against Facebook budget on 200 included observations.

## Results
Advertising regression achieved R²=0.9464 on its fitting data and predicted approximately $71,830 in sales for a $50,000 budget. For the illustrative confusion matrix (TN=100, FP=20, FN=120, TP=80), accuracy is 56.25%, precision 80%, recall 40% and specificity 83.33%. These are separate examples, not one evaluated classifier.

## Limitations
The linear_regression.joblib and logistic_regression.joblib files and their training workflows were absent. Their archived summaries remain available for interpretation, but those models cannot be reproduced from this repository. Advertising R² is in-sample with no held-out evaluation; association does not establish incremental advertising impact. Logistic effects concern odds, not probability, and balance units depend on undocumented preprocessing.

## Data
Data/marketing.csv contains 200 advertising-budget and sales observations, both expressed in thousands of USD according to the original notebook. Upstream dataset provenance is not documented. Vehicle and bank model examples are archived summaries rather than bundled fitted artifacts.

## Verification
Included-data code cells executed successfully during this update.

## Run
```bash
python -m pip install -r requirements.txt
jupyter lab
```
Open [the notebook](Notebooks/regression_classification_metrics.ipynb) and run cells in order. Dependencies are unpinned.

## Files
- [Analysis report](Reports/regression_classification_metrics.html)
- [Original PDF](Reports/regression_classification_metrics.pdf): historical export; may predate corrections.
- [Live portfolio report](https://cameron-batts.github.io/regression_classification_metrics.html)
