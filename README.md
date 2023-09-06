# Airbnb Data Visualization 
This repository showcases data visualization techniques using Tableau 
## Introduction 
For this project, I utilized data to understand revenue optimization of AirBnb rentals in the Seattle, WA area. 

Use case: Considering 3 important factors for ROI- location, peak rental months, and number of bedrooms of rental properties. 

Data Source [http://insideairbnb.com/get-the-data/](https://www.kaggle.com/datasets/alexanderfreberg/airbnb-listings-2016-dataset)https://www.kaggle.com/datasets/alexanderfreberg/airbnb-listings-2016-dataset

## Step 1- Download dataset in Excel 
3 sheets in workbook- listings, reviews, calendar

Review data in Excel to understand data being presented.
Listing sheet contains column "id" which corresponds to "listing_id" column in the Calendar sheet 
These are the columns we will use when joining the tables in Tableau. In the listing tab, price refers to amount rentals are charging per night and bedrooms refers to number of bedrooms in the rentals. In the calendar tab, price refers to how much the rentals cost on that specific date. 

## Step 2- Upload data to Tableau 
Uploaded Excel workbook to Tableau. Used inner join to join the listing and calendar datasets. Join by corresponding columns- "listing_id" and "id". Once tables are joined, we can start visualizing. 

<img width="366" alt="Screen Shot 2023-09-06 at 3 08 24 PM" src="https://github.com/Cthomas3067/AirBnb-Project/assets/144178514/eb519254-fc14-4061-8ff3-72b544c604d4">

## Step 3- Creating Visualizations to Answer Questions
Question 1 
Where is the best place to buy a home for AirBnb rentals? 
2 Visuals

Bar Graph- Using Listing dataset: Price (avg) for row (y-axis) and Zipcode for column (x-axis). Exclude all nulls for both price and zipcode. 

Region Mapping 
Using Zipcodes lattitude and longtitude 
Add price(avg) as a label to showcase the how much rentals are priced at based on location.


Based on this data, we can say that rentals in zipcode 98134 have the highest avg list price per night compared to other zipcodes. This suggests if you were to buy a home in zipcode 98134, you could charge a higher rate per night than if you bought a rental in another zipcode. 





