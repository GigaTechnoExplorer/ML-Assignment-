# ML Assignment: Wine Quality Prediction

## What is the dataset about?

The WineQT dataset from Kaggle has 1,143 wines described by 11 chemical measurements (alcohol, volatile acidity, sulphates, etc.) and a quality score from 3 to 8.

## What are you predicting?

Whether a wine is "Good" (quality ≥ 6) or "Not Good" (quality ≤ 5) from its chemical properties. I also predicted the numeric quality score and checked which chemicals matter most.

## Which models did you use?

Logistic Regression, Random Forest and Linear Regression.

## Your results

Random Forest had the best test accuracy (81.2%, F1 0.83) but scored 100% on the training data, so it overfits. Logistic Regression scored 77.7% (5-fold CV accuracy 74.4%) and Linear Regression 78.6% (R² = 0.39 on the quality score).

## What did you learn?

Principles and application of multicollinearity.
A model that looks best on one train/test split is not necessarily the best. Random Forest won on the test set, but cross-validation put it behind logistic regression (72.9% vs 74.4%), so I now check overfitting and use cross-validation before comparing models.



