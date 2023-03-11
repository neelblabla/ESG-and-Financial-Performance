# ESG and Financial Performance

Hey there!

We are a team of data science master students at Frankfurt School of Finance and Management. In this project we investigate the relationship between ESG factors and (financial) firm performance. Our final cleaned dataset consists of 6.946 individual firms with data across twenty years. Availability varies, so we end up with 50.736 observations in total.

After we validated our data and completed an EDA, we proceeded to fit ML-Models conditioned on different aspects like company size, region or industry. Our findings are in line with literature (https://www.sciencedirect.com/science/article/pii/S0929119921000092?via%3Dihub), alltough we were able to work out some interesting insights.

### Regression

Contrary to our hypothesis, financial performance seems to be indicative of ESG performance

Explanatory power is limited however, with R2 values of around 0.2

This might be indicative of companies with sound financials being able to spend more on their ESG initiatives

This is supported by the fact that large companies have higher ESG scores on average than small cap contestants

### Classification

Here our hypothesis is confirmed – movements in ESG can indeed be indicative of movements in financial metrics

The dataset is skewed towards positive returns, which impacts the accuracy of our models

YoY changes in ESG seem to be a better indicator of subsequent movements in financial metrics than same year absolute values

Robustness of the results is ensured by training the models for 100 iterations, each time on randomly split training and test sets


### Description of folders:

1) Data Collection and Preparation -> Retrieving data from the Refinitiv Workspace Python API and steps that are needed to build our final dataset, combining general company information, ESG and financial data

2) Analysis -> EDA, Regression + Classification Modelling for in-depth hypthesis testing using Random Forest

3) Data -> Storage of all datasets that have been created during the project
