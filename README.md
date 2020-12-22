# Boston Airbnb Dataset

## How much should you price your Boston Airbnb?

We take a look at Airbnb data for Boston to provide potential hosts with an idea for the sort of prices they should be charging.

We depend mostly on Linear Regression to provide a simple formula for estimating the price hosts should be charging. Random Forests and XGBoost then provide more flexible methods for accounting for the variance in the data and double checking the important features.

Key features in deciding the price:

- Number of bedrooms and bathrooms
- Whether the listing is for a shared or private room or the whole place
- The neighbourhood

We account for 90% of the variability in the data using the ensemble methods but still with a significant root-mean-squared-error. We end on the note that while the models do a great job of generalizing prices based on features, each listing is unique and it's impossible to capture what makes a traveller decide that a place is worth the money.

These findings are posted on both [Kaggle](https://www.kaggle.com/ryanfox212/how-much-should-you-price-your-boston-airbnb) in a kernel and on my website at [rfoxdata.co.uk](https://rfoxdata.co.uk/general/python/2020/12/22/what-price-to-charge-for-your-airbnb.html)

## Running the notebook

Package requirements have been listed in `requirements.txt` with the notebook mainly leverages pandas and sklearn for the analysis.

It's recommended to create a virtual environment before running the notebook using the

```
conda create -n newEnv
conda activate newEnv
pip install -r requirements.txt
```

## Acknowledgements

The dataset came through [Kaggle](https://www.kaggle.com/ryanfox212/how-much-should-you-price-your-boston-airbnb) but can be accessed directly from [Airbnb](http://insideairbnb.com/get-the-data.html).
