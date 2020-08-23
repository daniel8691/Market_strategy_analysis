# KPMG-virtualinternship

Visualizations for this project can be better viewed on [Tableau Public](https://public.tableau.com/profile/daniel8010#!/vizhome/KPMGMarketingStrategyDataAnalysis/Story1)


## Module One: Data Quality Assessment
### Problem Statement
Sprocket Central Pty Ltd , a medium size bikes & cycling accessories organisation, has approached Tony Smith (Partner) in KPMG’s Lighthouse & Innovation Team. Sprocket Central Pty Ltd  is keen to learn more about KPMG’s expertise in its Analytics, Information & Modelling team. 

Smith discusses KPMG’s expertise in this space (you can read more here). In particular, he speaks about how the team can effectively analyse the datasets to help Sprocket Central Pty Ltd grow its business.

Primarily, Sprocket Central Pty Ltd needs help with its customer and transactions data. The organisation has a large dataset relating to its customers, but their team is unsure how to effectively analyse it to help optimise its marketing strategy. 

However, in order to support the analysis, you speak to the Associate Director for some ideas and she advised that “the importance of optimising the quality of customer datasets cannot be underestimated. The better the quality of the dataset, the better chance you will be able to use it drive company growth.”

The client provided KPMG with 3 datasets:

Customer Demographic 
Customer Addresses
Transactions data in the past 3 months
You decide to start the preliminary data exploration and identify ways to improve the quality of Sprocket Central Pty Ltd’s data.


### My Work
**Missing Data**

I started this module by loading the excel sheet containing all the datasets onto Jupyter Notebook for data cleaning and manipulation. The "Transaction" worksheet contained missing values but the missing values only represented for around 2% of the total data so I simply removed the missing data.

**Inconsistent Values**

I noticed that there are inconsistent values for the same attribute. For instance, within the gender column, there are three different values for Females (F, Femal, Female) and two different values for Males (M, Male). Another issue was the "States" column where the state, Victoria, was represented as "V", VIC", and "Victoria". A possible solution is to use "Drop Down List" formats for data entries to ensure data entry consistency. 

**Inconsistent DataTypes**

There were inconsistent datatypes for some features in the datasets. For example, a feature contained string datatypes, datetime objects and integers all within one column. A solution to mitigate this issue could be setting contraints on the data attribute to either string or interger/float. 

**Data Accuracy**

Part of the data quality assessment was to check the accuracy of the data to make sure all the data make sense. I checked the DOB (date of birth) feature and found that a person had a DOB value of 1843 which means the person is now over 150 years old which obviously was an error within the dataset.

**Inconsistent customer_id Accross Datasets**
Additional customer_ids were found in the transactions table and customer address table but not in the master customer table. This may be caused data received at different time periods which may skew the data. 

## Module Two: Data Insights and Presentation
### Problem Statment
For context, Sprocket Central Pty Ltd is a long-standing KPMG client whom specialises in high-quality bikes and accessible cycling accessories to riders. Their marketing team is looking to boost business by analysing their existing customer dataset to determine customer trends and behaviour. 

Using the existing 3 datasets (Customer demographic, customer address and transactions) as a labelled dataset, please recommend which of these 1000 new customers should be targeted to drive the most value for the organisation. 

In building this recommendation, we need to start with a PowerPoint presentation which outlines the approach which we will be taking. The client has agreed on a 3 week scope with the following 3 phases as follows - Data Exploration; Model Development and Interpretation.

Prepare a detailed approach for completing the analysis including activities – i.e. understanding the data distributions, feature engineering, data transformations, modelling, results interpretation and reporting. This detailed plan needs to be presented to the client to get a sign-off. Please advise what steps you would take. 

Please ensure your PowerPoint presentation includes a detailed approach for our strategy behind each of the 3 phases including activities involved in each - i.e. understanding the data distributions, feature engineering, data transformations, modelling, results interpretation and reporting. This detailed plan needs to be presented to the client to get a sign-off.


### My Work

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")


