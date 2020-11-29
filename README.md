## MSBD5001 - Individual Project

### Programming Language
* Python 3.7+

### Packages Used
This section has listed out tha major packages used for data wrangling and model building in this project. Program code for importing/installing the necessary packages has been included in the attached Jupyter Notebooks. The Jupyter Notebooks attached have been tested in Kaggle/Google Colab with no problem found per execution.

* Beautiful Soup  (https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
* NumPy           (https://numpy.org/doc/stable/)
* Pandas          (https://pandas.pydata.org/)
* scikit-learn    (https://scikit-learn.org/stable/)
* Selenium        (https://selenium-python.readthedocs.io/)
* urllib          (https://docs.python.org/3.7/library/urllib.html)
* XGBoost         (https://xgboost.readthedocs.io/en/latest/index.html)

### Dataset used

* Traffic Speed Dataset provided in Kaggle\ (https://www.kaggle.com/c/msbd5001-fall2020/data)
* Hong Kong Public Holiday Data from GovHK (香港政府一站通)\ (https://www.gov.hk/en/about/abouthk/holiday/)
* Rainfall Data Scraped from Hong Kong Observatory\ (https://www.hko.gov.hk/en/cis/dailyExtract.htm?y=2020&m=10)

### Submitted Jupyter Notebooks

1. Scraping of Rainfall Data from HKO\
   This notebook has included the program code for extracting historical rainfall record of Hong Kong during the period 2017-2018 from Hong Kong Observatory.

2. Road Speed Prediction (baseline)\
   Exploratory data analysis has been done in this notebook to search for factors that are influential to average traffic speed through visualization (mainly line graph and box plot). A baseline model is then built by dividing the training data into different groups by the important factors identified in exploratory analysis, and then taking the median traffic speed of each group. Median is chosen as estimator as it is more robust and should be less affected by outliers.

3. Road Speed Prediction (xgboost)\
   In this notebook, a gradient boosted tree has been trained for doing the prediction. The final submission made in Kaggle is generated from this notebook.


### Model Comparison

* Kaggle Score (MSE) of the baseline model: 15.04727
* Kaggle Score (MSE) of the xgboost model: 10.76706