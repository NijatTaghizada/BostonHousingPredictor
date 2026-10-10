# Boston Housing Price Predictor

A random forest model that predicts median house prices (`medv`) from the classic Boston Housing dataset.

What the notebook does:

- looks at the data, e.g. number of rooms vs. price
- removes outliers (rows with any feature more than 3 standard deviations from the mean)
- trains a random forest with 100 trees on 60% of the data and tests on the other 40%

It got an R² of about 0.81 on the test set.

At the end I also tried adding synthetic rows generated from each feature's distribution. That made the score worse (about 0.70), so the original model is the better one.

## Run it

```bash
pip install numpy pandas scikit-learn matplotlib seaborn
jupyter notebook HousePricePredictor.ipynb
```
