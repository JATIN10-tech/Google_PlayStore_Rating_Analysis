# Google_PlayStore_Rating_Analysis
## EDA & Data Preprocessing on Google App Store Rating Dataset.

## Domain: Mobile device apps
![alt text](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQSkTGQmxNUhGygUg56uPhufOSsHi3OEsWruQ&s)

## Context:
The Play Store apps data has enormous potential to drive app-making businesses to success. However, many apps are being developed every single day and only a few of them become profitable. It is important for developers to be able to predict the success of their app and incorporate features which makes an app successful. Before any such predictive-study can be done, it is necessary to do EDA and data-preprocessing on the apps data available for google app store applications. From the collected apps data and user ratings from the app stores, let's try to extract insightful information.

## Objective:
The Goal is to explore the data and pre-process it for future use in any predictive analytics study.

## Data Dictionary
![alt text](https://private-user-images.githubusercontent.com/130181481/237484177-c8ae54cf-2f04-49a1-9bb2-14d5c9b1ec34.png)
![alt text](https://private-user-images.githubusercontent.com/130181481/237484258-cdd7d629-38a3-443b-91d8-b4e487bf51e2.png)

## Questions:
- Q1) Import required libraries and read the dataset.
- Q2) Check the first few samples, shape, info of the data and try to familiarize yourself with different features.
- Q3) Check summary statistics of the dataset. List out the columns that need to be worked upon for model building.
- Q4) Check if there are any duplicate records in the dataset? if any drop them.
- Q5) Check the unique categories of the column 'Category', Is there any invalid category? If yes, drop them.
- Q6) Check if there are missing values present in the column Rating, If any? drop them and and create a new column as 'Rating_category' by converting ratings to high and low 
      categories(>3.5 is high rest low)
- Q7) Check the distribution of the newly created column 'Rating_category' and comment on the distribution.
  Convert the column "Reviews'' to numeric data type and check the presence of outliers in the column and handle the outliers using a transformation approach.(Hint: Use log 
  transformation)
- Q8) Convert the column "Reviews'' to numeric data type and check the presence of outliers in the column and handle the outliers using a transformation approach.(Hint: Use log 
      transformation)
- Q9) The column 'Size' contains alphanumeric values, treat the non numeric data and convert the column into suitable data type. (hint: Replace M with 1 million and K with 1 thousand, 
      and drop the entries where size='Varies with device')
- Q10) Check the column 'Installs', treat the unwanted characters and convert the column into a suitable data type.
- Q11) Check the column 'Price' , remove the unwanted characters and convert the column into a suitable data type.
- Q12) Drop the columns which you think redundant for the analysis.(suggestion: drop column 'rating', since we created a new feature from it (i.e. rating_category) and the columns 'App',        'Rating' ,'Genres','Last Updated', 'Current Ver','Android Ver' columns since which are redundant for our analysis)
- Q13) Encode the categorical columns.
- Q14) Segregate the target and independent features (Hint: Use Rating_category as the target)
- Q15) Split the dataset into train and test.
- Q16) Standardize the data, so that the values are within a particular range.
