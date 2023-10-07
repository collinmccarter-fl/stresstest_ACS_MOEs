## Stress Testing Machine Learning Projections with ACS MOEs

_Southern Demographic Association Annual Meeting_
<br>
_October 20th, 2023_
<br>
_by Collin McCarter_
<br>
_https://www.linkedin.com/in/collin-mccarter/_
<br>
_https://github.com/flolabs-cm_
<br>

* 2022 - TODAY ... Data Science, Northwestern Mutual
* 2020 - 2022  ... Technology & Product Management, Trellance (Credit Unions)
* 2016 - 2020  ... Demographer, Nielsen (TV Ratings)
* 2014 - 2016  ... PK-12 School Enrollment Analyst, State of Florida

------------------------

**ABSTRACT:**

A common private sector use case for ACS data is to link ACS data with a “client dataset” by small-area geography to improve predictive performance of a machine learning model. Model objectives can vary widely by sector and data sources, but the ubiquity of machine learning models using ACS estimates is clear. In my experience, ML experts who are strong in methods tend to disregard data uncertainty (MOEs), which poses problems when using ACS estimates with high MOEs. This presentation will demonstrate Python code pulling data from the US Census API to stress test 4 different machine learning models trying to predict if a county will gain population in the next year. Extending MOE best practices to ML methods will likely prove to be a fruitful research topic as survey estimates are leveraged as predictors by ML practitioners.

* Organizations **link ACS data with a “client dataset”** by small-area geographies
* Organizations are always searching for **"new data sources"** to differentiate the organization
* Discovering "new data sources" comes with a **learning curve**
* ACS MOE's can be a **time consuming learning curve** for big data practioners, especially those without a survey background
* **Stress testing examples** may help to lessen the learning curve, which is possible with MOE-adjusted ACS variables
------------------------
**AGENDA:**

Highlight key areas of this Jupyter Notebook, which perform the following tasks to **stress test** machine learning models with ACS MOEs:

* Gather packages of functions (aka procedures) from PIP
* Pull select api.census.gov data, ACS 1yr Data Profile
* Pull select api.census.gov data, PEP Vintage 2010
* Pull select api.census.gov data, PEP Vintage 2020
* Pull select api.census.gov data, PEP Vintage 2022
* Transform and Merge US Census data into a training dataset for machine learning packages
* Train (fit), Predict, and Evaluate different projects based on below adjustments:
    * ACS variables used as predictive features vs univariate timeseries
    * Adjusted ACS variables using MOEs vs ACS variable point estimates
    * Continuous Regression metrics (MAE, MSE, MAPE, r^2)
    * Models available on PIP (structureboost, statsforecast, catboost)
------------------------
**TLDR:**

1. This notebook runs start to finish in ~5min on my MacBook Pro ...
    * these tools are efficient, accessible, and reproducible but are not frequently used in applied demography
2. PIP packages are maturing in their documentation, peer-review credibility, and flexible options.
3. Machine Learning practicioners are using these tools and data without domain knowledge and getting mixed results.

##### Applied Demographers have the domain knowledge to maximize value from these tools for decision makers

SO LET'S LEARN HOW THESE NEW TOOLS CAN IMPROVE YOUR DATA WORKFLOW
------------------------

Feel free to reach out on LinkedIn for any data digression!
