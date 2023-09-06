# Airbnb Data Visualization 
This repository showcases data visualization techniques using Tableau. 
## Introduction 
For this project, I utilized data to understand revenue optimization of AirBnb rentals in the Seattle, WA area. 

**Use case**: Individual would like to purchase and rent an AirBnb in Seattle, WA. 

Considering 3 important factors for ROI- location, peak rental months, and number of bedrooms of rental properties. 

### Ask 
1. Which area can you charge the most for AirBnb rentals?
2. What are the peak months for Airbnb rentals?
3. How does the number of bedrooms affect price of rental? 


## Data Exploration

Data Source [http://insideairbnb.com/get-the-data/](https://www.kaggle.com/datasets/alexanderfreberg/airbnb-listings-2016-dataset)https://www.kaggle.com/datasets/alexanderfreberg/airbnb-listings-2016-dataset


Three sheets in Excel workbook- listings, reviews, calendar. We are focusing on listings and calendar for this project. 

Review data in Excel to understand data being presented.
Listing sheet contains column "id" which corresponds to "listing_id" column in the Calendar sheet. 
These are the columns we will use when joining the tables in Tableau. In the listing tab, price refers to amount rentals are charging per night, zipcode refers to zipcode rental is located in, and bedrooms refers to number of bedrooms in the rentals. In the calendar tab, price refers to how much the rentals cost on that specific date. 

## Data Visualization
Uploaded Excel workbook to Tableau. Used inner join to join the listing and calendar datasets. Join by corresponding columns- "listing_id" and "id". Once tables are joined, we can start visualizing. 

<img width="366" alt="Screen Shot 2023-09-06 at 3 08 24 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/eb519254-fc14-4061-8ff3-72b544c604d4">

&nbsp;

Now we can create visuals based on the dataset. The first two visualizations aim to answer the first question: Which area can you charge the most for AirBnb rentals?

<img width="500" alt="Screen Shot 2023-09-06 at 3 23 32 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/51e9fa41-636e-4d02-af96-01307b93b692">

> **_Bar Graph- Using Listing dataset: Price (avg) for row (y-axis) and Zipcode for column (x-axis). Exclude all nulls for both price and zipcode._**

&nbsp;
<img width="500" alt="Screen Shot 2023-09-06 at 3 24 27 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/8c7c2597-8caa-4bc0-bc24-aa9364d14d06">

> **_Region Mapping- Using listing zipcodes' latitude and longitude. Add price(avg) as a label to showcase the how much rentals are priced based on location.Exclude all nulls for both price and zipcode._**


**Based on this data, we can say that rentals in zipcode 98134 have the highest avg list price per night compared to other zipcodes. This suggests if you were to buy a home in zipcode 98134, you could charge a higher rate per night than if you bought a rental in another zipcode.**


This visualization analyzes how price changes over time in order to answer the second question: What are the peak months for Airbnb rentals?

<img width="500" alt="Screen Shot 2023-09-06 at 3 48 25 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/5c619f8d-7aa0-4dd5-bc72-0e9e67a370bd">


> **_Line Graph- Using weeks in 2016 as x-axis to showcase avg price changes. Exclude all nulls for price._**

**Based on 2016 data, over the summer and at the end of the year are peak seasons for Airbnb rentals in Seattle, WA.**

Now we want to answer our third and final question: How does the number of bedrooms affect price of rental? 
This visualization shows the avg price of the rentals based on the number of bedrooms. 


**For 5 and 6 bedroom rentals, there is a higher return on investment compared to smaller rentals with fewer bedrooms.**

We can dive further into the data to understand the competition in the 5 to 6 bedroom market. 

> **_Bar Graph- Count of bedrooms by avg price. Exclude all null and 0 bedroom listings._**

Here we can see the count of rental listings by number of bedrooms. As we can see, there are far fewer listings that have 5 to 6 bedrooms i.e less competition in that market. 

> **_Table- Number of rental listings per number of bedrooms. Exclude all null and 0 bedroom listings._**


