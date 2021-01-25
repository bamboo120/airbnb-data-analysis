# airbnb-data-analysis


## Business Understanding

1: Based on the data, what is the most polular size for the host place (like how many beds host are provided)?

2: Based on the data, what is the most popular price?

3: What feathers affect the review score rating?

## Data Understanding

1: We can check the histogram and the mean value of beds.

2: We can check the histogram and the mean value of price.

3: I pick some related feathers affected the review score rating below: 'cancellation_policy','guests_included','host_response_time','host_response_rate','host_acceptance_rate','host_has_profile_pic','host_identity_verified','room_type','accommodates','bathrooms','bedrooms','beds','bed_type','price','number_of_reviews','review_scores_rating','instant_bookable','reviews_per_month','review_scores_value','review_scores_location','review_scores_communication','review_scores_checkin','review_scores_cleanliness','review_scores_accuracy'

## Prepare Data

1: the data of beds is ready

2: the price need to change into float

3: except of review score rating, the int and float data NAN are replaced with the mean value. And dummy the categorical variables 

## Data Modeling

Split training and testing data. Use 'review_scores_rating' as y, the rest feathers as X. Apply linear regression to learn the data.

## Evaluate the Results


![alt text](https://github.com/bamboo120/airbnb-data-analysis/blob/main/Seattle_beds.png "Seattle Airbnb beds")![alt text](https://github.com/bamboo120/airbnb-data-analysis/blob/main/Boston_beds.png)

Up one: Seattle beds histogram Down: Boston beds histogram

## Summary the Results

1: The popular size are 1-2 beds for host

2: The popular price is around $100

3: The top feathers affects the review score rating are:

- Keep your place clean
- describe your place accurate
- communication, response in time
- make yourself look reliable, like providing a nice host picture
- easy check-in
- nice bed
- good location

## File description: 
All the data is in Archive.zip
In Archive.zip, boston.csv is the data of Airbnb price and data in Boston. seattle.csv is the data of Airbnb price and data in Seattle.
list_boston.csv is the feathers of airbnb in Boston. list_seattle.csv is the feathers of airbnb in Seattle. 

The code price1.ipynb is to calculate the price histogram and the beds histogram in Boston and seattle.
The code correlation.ipynb is to calculate the correlation of feathers.
The code top10feather.ipynb is aim to test the top 10 feather affect the review score.

## python library

numpy

pandas

matplotlib.pyplot

sklearn

seaborn

## acknowledgments

This is Udacity data science nano degree project. The data is from kaggle [Boston Pages](https://www.kaggle.com/airbnb/seattle/data) [Seattle Pages](https://www.kaggle.com/airbnb/boston)
