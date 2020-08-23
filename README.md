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

Some key questions to answer are:
* What are the trends in the underlying data?
* Which customer segment has the highest customer value?
* What do you propose should be Sprocket Central Pty Ltd ’s marketing and growth strategy?
* What additional external datasets may be useful to obtain greater insights into customer preferences and propensity to purchase the products?


### My Visualizations

<hr>

![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/new_customer_age_groups.png)
![old customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/old_customer_age_groups.png)
We can see that most customers age around 40-49 years old. The least popular groups are 10-19 and 70 years old and above.
In general, the most popular shoppers tend age between 20 to 69 years old. 
<hr>

![customer gender past 3 year purchases pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/new_customer_bike_related_purchases_for_the_past_3_years_by_gender.png)
Customer gender demographic is evenly spread among males and females, however, females make up majority of the bike purchases by a slight margin

<hr>

![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/new_wealth_segment_by_age.png)
![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/old_wealth_segment_by_age.png)
Most customers are classified as "Mass Customer". Other niche markets includes "High Net Worth" and "Affluent Customers" they behave similarly but we can see that high net worth customers tend to purchase from the business more than affluent customers. 

<hr>

![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/new_job_industry_category_distribution.png)
![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/old_job_industry_category_distribution.png)
The top three industries that customers work in are Financial Services, Manufacturing, and Health sections respectively. The least popular job industries are Telecommunications, Agriculture, Entertainment and IT. 

<hr>

![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/new_customers_number_cars_own_per_state.png)
![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/old_customers_number_cars_own_per_state.png)

Most customers from New South Wales do not own a vehicle while most customers from Queensland (QLD) and Victoria (VIC) own a vehicle. Which customer should we target?
![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/profitability%20between%20age%20groups.png)
This graph shows the people who own vehicles tend to be more profitable across all age groups so from these three charts, we can choose to target states that have higher car ownership rates.

<hr>

### RFM Analysis (Recency, Frequency, Monetary)
![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/customer_title_description_df.jpg)
* RFM measures customers' behavior. 
* Frequency and Monetary affects customer lifetime value
* Classified into four groups by their RFM score from highest to lowest respectively: Platinum, Gold, Silver, and Bronze

![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/RFM%20Analysis.png)
The graph in the top left cornor describes the relationship between Recency and Profitability (Monetary). We can see that Platinum customers are the customers who tend to buy more recently and spent the most money. There is a negative correlation between recency and monetary meaning that the less recent the last purchase is, the customer will likely to spend less.

The graph in the bottom left cornor shows the relationship between recency and frequency. We can see that platinum customers tend to buy more recently and frequently than other groups. There is a negative correlation between recency and frequency, meaning that the less recent the last purchase is, the customer will likely buy less frequently.

The graph on the right shows describes the relationship between frequency and monetary. Platinum and gold customers scatters around the right side, which indicates that they purchase more frequently than other customer groups. We can see a positive correlation trend that implies that a customer is more likely to be more profitable, the more frequently the customer buys. 

### Conclusion
![customer age group pic](https://github.com/daniel8691/KPMG-virtualinternship/blob/master/Module_two/ppt_graphs/top_1000_customers.jpg)

This is the chart of the top 1000 customers Sprocket Central could target. This list is ranked based on the customer's RFM score as customers who have high RFM scores tend to be the most valuable customers for the business. 

To summarize the findings from this analysis:
* Most of the customers for Sprocket work in financal services, manufacturing and health sectors. 
* Most customers who make purchases at Sprocket are aged between 40 to 49 years old. 
* Customers who own a vehicle tend to be the more profitable customers in terms of average profit generated for the customer.






