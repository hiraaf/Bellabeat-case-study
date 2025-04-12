# Bellabeat-case-study

## Kaggle
Code also available in [Kaggle](https://www.kaggle.com/code/hiraaf/bellabeat-case-study#Background)

## Background

Bellabeat is a high-tech manufacturer of health-focused products for women. The objective is to analyze Bellabeat's product into gaining insight on how consumers are using their smart devices. The analysis will be used to make high-level recommendations for marketing strategy.

The questions that should guide the analysis are:   
1. What are some trends in smart device usage?    
2. How could these trends apply to Bellabeat customers?   
3. How could these trends help influence Bellabeat marketing strategy?   

## Data source

Bellabeat data was taken from [*FitBit Fitness tracker Data*](https://www.kaggle.com/datasets/arashnic/fitbit)

License: [*CC0: Public Domain*](https://creativecommons.org/publicdomain/zero/1.0/)    
Data set made available through Mobius

Data is generated from eligible Fitbit users who consented to the use of their personal tracker data that includes physical activity, sleep, calories etc...        
Data is dated from 03-12-2016 to 05-12-2016

## Data Exploration
- Identify duplicate records in data 
- Identify null values in data 
- Cross-reference users between daily_activity datasets to identify users missing from either datasets 
- Cross-reference users between hourly_steps and hourly_intensities datasets to identify users missing from either datasets 
- Cross-reference users between minute_sleep and weight datasets to identify users missing from either datasets 

## Data Combining and Cleaning
- Combine mar_apr_daily_activity and apr_may_daily_activity for users that exist in both data sets. Convert ActivityDate field from char to Date. 
- Combine mar_apr_hourly_activity and apr_may_hourly_activity for users that exist in both data sets. Convert ActivityHour field from char to Date. Create separate column to store date and hour from ActivityHour column. 
- Remove duplicated records from both datasets. Sum each users total sleep (filter value to 1 which is indication that user is asleep) and store it as a separate column. Convert date field from char to Date. Generate separate date column from date (mdy_hms) field. Combine both datasets. 
- Combine March - April and April - May weight data set. 

## Data Visualization and Analysis    
- Identify trend of how consistent user was in wearing Fitbit across the 2 months by analyzing how many days with zero steps each user had:
- Identify trend of how consistent user was in wearing Fitbit across the 2 months by analyzing how many days with zero steps each user had across the week:
- Identifying user engagement pattern by measuring conversion rate from wearing Fitbit device to user logging sleep and weight data
- Analyzing users weekly physical activity trends by variations in step count across weekday 
- Analyzing users activity levels by average time spent very active, fairly active and lightly active
- Analyzing users weekly physical activity trends by variations in step count across 24 hours
- Analyzing users sleep duration pattern across the weekday
- Asses sleep tracking of users by computing the average number of daily sleep recording across user

# Recommendations
- Streaks, Rewards, and Premium
- Introduce Low Effort Weight Tracking
- Encourage Sleep Monitoring
- Physical Activity 
