# CFPB_complaint_disputes
In this project I built a supervised learning model to predict the escalation of CFPB complaints

### Requirements

Python: pandas, scikit-learn, numpy, scipy, jupyter ntoebook  

PostgreSQL (optional)

### Details

Data was collected from the [CFPB Complaint Database](https://www.consumerfinance.gov/data-research/consumer-complaints/) and the [CFPB Survey of credit card agreements](https://www.consumerfinance.gov/data-research/credit-card-data/).

`data_clean_for_sql.ipynb`: Cleans credit card data so it can be uploaded to a PostgreSQL database

`data_explore.ipynb`: Most of the work is done in this file.  Data is pulled from the PostgreSQL database, cleaned and processed, then passed to a learning model.

### Results

The model with the best performance was a Gradient Boosting Learner, with a test AUC of approximately 0.64.
