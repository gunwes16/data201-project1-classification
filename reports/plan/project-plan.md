# Project 1 Plan: Predicting Term Deposit Subscriptions

## Question
Can I predict which bank clients will subscribe to a term deposit
after a marketing campaign, and which classification method is best?

## Data
- Source: Bank Marketing dataset (bank-full.csv)
- Size: 45,211 clients, 17 columns
- Target: `y` — 1 = subscribed, 0 = did not
- Positive class: subscribed

## Predictors
- Client: age, job, marital, education, default, balance, housing, loan
- Campaign: contact, day, month, campaign, pdays, previous, outcome
- Excluded: duration — call length is only known after the call ends,
  so using it would leak the outcome into the model

## Methods
Logistic regression, LDA, QDA, KNN

## Evaluation
- Confusion matrix, accuracy, precision
-Baseline to beat: accuracy from always predicting the majority class ("no"), computed in notebook
