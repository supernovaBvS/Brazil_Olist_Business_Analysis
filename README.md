# Brazil_Olist_Business_Analysis

## Brief
Olist Store is the largest department store in Brazilian marketplaces. Olist connects small businesses from all over Brazil to channels without hassle and with a single contract. The Brazilian ecommerce public dataset of orders (from 2016 to 2018) made at Olist Store is provided to your company for analysis.

Your manager is asking you to critically analyse the provided datasets using Business Intelligence tools and provide some marketing findings / recommendations in a report format. The dataset has information of 100k orders made at multiple marketplaces in Brazil. Its features allow viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. A geolocation dataset that relates Brazilian zip codes to lat/lng coordinates is also integrated in the dataset.

After a customer purchases the product from Olist Store, a seller gets notified to fulfill that order. Once the customer receives the product, or the estimated delivery date is due, the customer gets a satisfaction survey by email where they can give a note for the purchase experience and write down some comments.

## Data Scheme
![database scheme](https://user-images.githubusercontent.com/112676063/205305572-374e80cd-da25-47d9-b03a-f716d0872d45.png)

## Objective
1. Create data pipeline to ingest data in PostgreSQL or SQL server database
2. Use Power BI to answer following questions:
  * How many customers, orders, and orders per customer does the company have?
  * What is the number of customers by state?
  * What is the number of orders by month?
  * What are the top 5 product categories?
3. Visualise the company’s customers’ demographics, sales trend, orders by categories, orders changes by year, etc. and use Power BI to help make better decisions
4. Map and compare report data with data from database query to validate the reports (functional testing).
5. Critically analyse relevant data using statistical methods (e.g., Predictive Modelling or Machine Learning)
6. Provide some recommendations and improvements (please refer to point 3 in the project description)

## Data Cleaning
Use Clean.ipynb to clean most of the wrong data type
* If city name have weird char => change to english
* são paulo -> sao paulo
* use value_counts() for knowing whats important for us to use in analysis

Put category from portuguese to english using translation file 
Such as dropna, unreasonable time and date
If product name, category = NAN jau drop

### SQL Database:
* PostgreSQL

## Machine Learning
 
### Machine Learning:(Classification)
* Deliver date - Order date
* Review score
* Sentiment 

### Sentiment Analysis:
* Nltk , transformers(huggieface)

## PowerBi Dashboard
olist home

![olist home](https://user-images.githubusercontent.com/112676063/205306712-ab8e4128-9b15-463e-ac1a-37abdc1e1ecf.png)

olist_stats

![olist_stats](https://user-images.githubusercontent.com/112676063/205306770-307e820a-f5ef-445a-81c5-b209232f923d.png)

olist_sentiment

![olist_sentiment](https://user-images.githubusercontent.com/112676063/205306785-dc71065d-2b11-4f32-b242-24b8accb9c82.png)

olist_comment of sentiment

![olist_comment](https://user-images.githubusercontent.com/112676063/205306800-5f65d683-af69-4639-a2d0-8aa1d488c866.png)

olist_forecast

![olist_forecast](https://user-images.githubusercontent.com/112676063/205306811-3224ce77-0ec2-45f6-b68a-2ef0e98ea0d4.png)

## Contributers
- Norton Wong
- Hollis Ho
- Louis Choi
- [Allen Kong](https://www.linkedin.com/in/allen-kong-21568b250/)
