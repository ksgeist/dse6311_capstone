# README

## Dataset description
This dataset captures anonymized subscription, transaction, and listening-activity records for customers of KKBox, a Taiwanese music streaming service, who donated a benchmark dataset for the WSDM (ACM International Conference on Web Search and Data Mining) Churn Prediction Challenge. The dataset contains real-world, granular, longitudinal transactional logs of multi-period user interactions up to March 31, 2017. Unlike traditional cross-sectional customer datasets, this dataset contains dynamic behavioral trajectories, including sequential updates to subscription lengths, plan downgrades/upgrades, pricing changes, and explicit cancellation actions.

Primary uses could include:

- constructing customer-level longitudinal features from transaction and activity records
- predicting subscription churn using a defined prediction window
- comparing customer retention patterns across subscription and usage histories
- evaluating time-aware model validation and the risk of temporal leakage

### Possible question
Which customers are likely to have the fastest churn, and does plan list price change (intervention) impact churn? (This question assumes that there are sufficient data points pre- and post-price change to be able to perform this exact prediction, however).

**Data access note:** The original competition data are distributed through Kaggle, and I could not verify a legitimate, complete non-Kaggle download source. This project is therefore provisional and should not be published as a no-Kaggle project until an acceptable distribution source is confirmed.

## Source Citation
KKBOX; WSDM Cup 2018. KKBox Churn Prediction Challenge. Mendeley Data. https://data.mendeley.com/datasets/mv3f8bdrvy/1

## Data documentation
The dataset is organized into member information, subscription transactions, daily listening logs, and churn labels. Another useful overview of the tables and their relationships is available in Databricks' instructional walkthrough: https://www.databricks.com/notebooks/churn/1-data-preparation.html

## Additional note
Real customer churn datasets are exceptionally rare. There are simulated datasets available, but this was the best real-world, granular churn set I could find as of this time. Thus, even though it goes against my, "shouldn't be part of a competition" rule, it's the only real option we have here without moving to simulated customer datasets.

Also, note that these files are quite large. I do not suggest putting them onto GitHub in their current state for this reason.
