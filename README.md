# Alphabet Soup Charity Analysis Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. We have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

- EIN and NAME — Identification columns
- APPLICATION_TYPE — Alphabet Soup application type
- AFFILIATION — Affiliated sector of industry
- CLASSIFICATION — Government organization classification
- USE_CASE — Use case for funding
- ORGANIZATION — Organization type
- STATUS — Active status
- INCOME_AMT — Income classification
- SPECIAL_CONSIDERATIONS — Special considerations for application
- ASK_AMT — Funding amount requested
- IS_SUCCESSFUL — Was the money used effectively

## Deliverables:
1. Preprocess the data
2. Compile, train, and evaluate the model
3. Optimize the model
4. Report, including overview and results

## Resources:
Data source: `charity_data.csv` <br>
Libraries used: `scikit-learn`, `pandas`, `tensorflow`

## Preprocessing:
1. Removed columns `EIN` and `NAME` which were non-beneficial as features
2. Binned the values in the `APPLICATION_TYPE` and `CLASSIFICATION` columns. Both columns had a large number of unique values, so reducing the number of unique values can help improve the performance of the model.
3. Split the data into the feature and target arrays
4. Scale the data using `StandardScaler`

## Compile, train, and evaluate the model:
Here, I experimented with different methods to optimize the model and achieve a predictive accuracy higher than 75%
The input data was adjusted using the following methods:
- Dropping more or fewer columns.
- Creating more bins for rare occurrences in columns.
- Increasing or decreasing the number of values for each bin.
- Add more neurons to a hidden layer.
- Add more hidden layers.
- Use different activation functions for the hidden layers.
- Add or reduce the number of epochs to the training regimen.
The desired predictive accuracy of 75% was not achieved, as I could only get an accuracy rating of 72.69%
