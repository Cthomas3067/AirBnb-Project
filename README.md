# Airbnb Data Visualization 
This repository showcases data visualization techniques using [Tableau](https://public.tableau.com/app/profile/christina.thomas8139/viz/AirBnbProject_16939502764760/Dashboard1#1)

## Introduction 
For this project, I utilized data to understand revenue optimization of AirBnb rentals in the Seattle, WA area. 

**Use case**: Stakeholder would like to purchase and rent an AirBnb in Seattle, WA. 

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

<img width="300" alt="Screen Shot 2023-09-06 at 3 08 24 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/eb519254-fc14-4061-8ff3-72b544c604d4">

&nbsp;

#### Now we can create visuals based on the dataset. The first two visualizations aim to answer the first question: Which area can you charge the most for AirBnb rentals?

<img width="800" alt="Screen Shot 2023-09-06 at 3 23 32 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/51e9fa41-636e-4d02-af96-01307b93b692">

> **_Bar Graph- Using Listing dataset: Price (avg) for row (y-axis) and Zipcode for column (x-axis). Exclude all nulls for both price and zipcode._**

&nbsp;
<img width="800" alt="Screen Shot 2023-09-06 at 3 24 27 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/8c7c2597-8caa-4bc0-bc24-aa9364d14d06">

> **_Region Mapping- Using listing zipcodes' latitude and longitude. Add price(avg) as a label to showcase the how much rentals are priced based on location.Exclude all nulls for both price and zipcode._**


**Based on this data, we can say that rentals in zipcode 98134 have the highest avg list price per night compared to other zipcodes. This suggests if you were to buy a home in zipcode 98134, you could charge a higher rate per night than if you bought a rental in another zipcode.**

&nbsp;

#### This visualization analyzes how price changes over time in order to answer the second question: What are the peak months for Airbnb rentals?

<img width="800" alt="Screen Shot 2023-09-06 at 3 48 25 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/5c619f8d-7aa0-4dd5-bc72-0e9e67a370bd">


> **_Line Graph- Using weeks in 2016 as x-axis to showcase avg price changes. Exclude all nulls for price._**

**Based on 2016 data, over the summer and at the end of the year are peak seasons for Airbnb rentals in Seattle, WA.**

&nbsp;

#### Now we want to answer our third and final question: How does the number of bedrooms affect price of rental? This visualization shows the avg price of the rentals based on the number of bedrooms. 


<img width="800" alt="Screen Shot 2023-09-06 at 4 49 24 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/05d54f5f-15ef-4f98-bd48-23daa0c06a1e">

> **_Bar Graph- Count of bedrooms by avg price. Exclude all null and 0 bedroom listings._**


**For 5 and 6 bedroom rentals, there is a higher return on investment compared to smaller rentals with fewer bedrooms.** &nbsp;

&nbsp;

We can dive further into the data to understand the competition in the 5 to 6 bedroom market. 


<img width="500" alt="Screen Shot 2023-09-06 at 4 58 34 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/b3b7ff43-ef68-473b-bb76-a1926150df7b">

> **_Table- Number of rental listings per number of bedrooms. Exclude all null and 0 bedroom listings._**


Here we can see the count of rental listings by number of bedrooms. As we can see, there are far fewer listings that have 5 to 6 bedrooms i.e. less competition in that market. 

### Dashboard 

We can put everything together in a dashboard to make data driven decisions and tell a story with data! 

![Dashboard 1](https://github.com/Cthomas3067/Portfolio/assets/144178514/77601c12-9c17-452a-9d44-0b63e733fe79)

## Act 

We can now make recommendations based on our data. 
1. According to our data analysis, rental properties within the 98134 zipcode exhibit the highest average rental rates in comparison to properties located in other zipcodes. To enhance revenue optimization, it would be strategically advantageous to consider property acquisition within the 98134 zipcode.

2. When considering seasonal rental strategies for residential properties, our analysis indicates that the optimal months for listing a property for rent are June, July, August, November, and December.

3. Our findings demonstrate that larger rental properties, characterized by an increased number of bedrooms, command higher average rental rates when contrasted with smaller rental units. As such, investing in a larger rental property may offer a more favorable return on investment (ROI), further augmented by reduced competition within the market segment of properties with multiple bedrooms.
