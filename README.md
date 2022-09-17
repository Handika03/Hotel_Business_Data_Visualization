# Hotel_Business_Data_Visualization
Data Visualization about customer characteristic in City Hotel &amp; Resort Hotel in certain period 

This is mini project from Rakamin Academy

## Overview

 - Dataset is obtained from [Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand) 
 - This data set contains booking information for a city hotel and a resort hotel, and includes information such as when the booking was made, length of stay, the number of adults, children, and/or babies, among other things.
 
## Data Preprocessing
Data has 29 columns and don't have major problem. Data null is very few and easy to handle. Columns `company` has the most missing value (data null) and I changed it into `unknown` value. The others data null I changed into 0.
 
## Feature Engineering
In feature engineering, I extracted new feature from the original feature to make it easier to analyze the dataset.
 
- `Stay_Duration` = `stays_in_weekend_nights` + `stays_in_weekdays_nights`
- `Total_Guests` = `adult` + `children` + `babies`

## Make histogram to show the difference of total booking each month
Data visualization of monthly hotel booking give us the information that the most total booking hotel is in June and July. My Recommendation is hotel management can give discount or promotion for other month except peak season (June and July). Discount can attract customer to booking the hotel.

## Make histogram to show the impact of stay duration on hotel booking cancellation rate
In this Data visualization we can get the insight that the cancellation rate is directly proportional to the stay duration. As the longer stay duration, the higher the percentage of booking hotel being cancelled. My recommendation is hotel management can make cancellation policy like cancellation charge. 

## Make histogram to show the impact of lead time on hotel booking cancellaation rate
In this visualization we can get the insight that the hotel have the lowest cancellation rate percentage in 1 month of lead time. City hotel has high cancellation rate above 70% with lead time around 10-12 months. And resort hotel has around 40% cancellation rate all the time. Probably the customer forget about their booking or they have important event in that time so they cancell their booking. This can be happened coonsidering the long lead time (10-12 month). My recommendation is hotel management can give reminder for customer. the reminder can be very useful to remind them. And hotel management can make cancellation policy like cancellation charge if customer cancel < 1 month before their booking date. 


