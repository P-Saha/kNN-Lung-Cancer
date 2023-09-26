# Analysis Plan for Datathon 1
## Preprocessing/feature Engineering
Prior to conducting analyses using both dataset, outliers that could potentially skew our results will be inspected and addressed to ensure high data quality. Based on visual inspection, there is no missing data in either dataset. Similar variables, such as height, weight and BMI, will be reduced to avoid redundancy and over-representation in the model-fitting process. This is also important to remove potential multicollinearity within the dataset. 

In addition, we are planning to:\
No missing data, so no problems to deal with in this regard\
Finding a pathway between BMI and obesity to be able to compare the two\
Label encoding for female and males\
Scaling for KNN and K-Means to ensure that higher ranges of data do not dominate (i.e. Caloric Intake for example)\
Remove multicollinearity from within the dataset, i.e. height and weight directly determine BMI\
Data Binning, i.e. turn the caloric intake continuous data into bins of 0-500, 501- 1000, 1001-1500, etc.

## KNN
Our plan is to try K-NN on both datasets to create a prediction model for the two datasets, where the response variables are BMI and Severity. The first KNN will look at the ethiopian data from this paper: (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10355424/) to predict the lung cancer severity based on multiple different predictors/factors including Age, Gender, Air Pollution, Alcohol Usage	, Genetic Risk,	Lung Disease,	Obesity, Smoking, whether they’re Passive Smokers, level of Chest Pain, Coughing of Blood in relation to the severity of lung cancer (which is labeled data ranging from 0-3, where low to 0, medium to 1, and high to 2. Three is the level assigned to healthy people.). As for the second dataset, we use data from statsCanada to predict the BMI level based on multiple different behaviors, and public health factors that may affect bmi. 

## K-Means
We are also interested in using K-Means Cluster analysis on both datasets, looking at their overlap in age, gender, and obesity/BMI. We will add a predictor based on which dataset each of the observations come from, and we hope to find clusters that correlate to various predictors within the datasets to see if there will be anything that may suggest possible inference or relationships within the clusters. For example, if we see that within a cluster, all of the points which are from the Cancer dataset also have a high genetic risk, this may perhaps suggest that the points within that cluster from the other dataset also have high genetic risk. 
