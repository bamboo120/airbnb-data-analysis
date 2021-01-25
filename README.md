# airbnb-data-analysis


## Business Understanding

1: Based on the data, what is the most polular size for the host place (like how many beds host are provided)?

2: Based on the data, what is the most popular price?

3: What features affect the review score rating?

## Data Understanding

1: We can check the histogram and the mean value of beds.

2: We can check the histogram and the mean value of price.

3: I pick some related features affected the review score rating below: 'cancellation_policy','guests_included','host_response_time','host_response_rate','host_acceptance_rate','host_has_profile_pic','host_identity_verified','room_type','accommodates','bathrooms','bedrooms','beds','bed_type','price','number_of_reviews','review_scores_rating','instant_bookable','reviews_per_month','review_scores_value','review_scores_location','review_scores_communication','review_scores_checkin','review_scores_cleanliness','review_scores_accuracy'

## Prepare Data

1: the data of beds is ready

2: the price need to change into float

3: except of review score rating, the int and float data NAN are replaced with the mean value. And dummy the categorical variables 

## Data Modeling

Split training and testing data. Use 'review_scores_rating' as y, the rest features as X. Apply linear regression to learn the data.

## Evaluate the Results

 ### most polular size for the host place
![alt text](https://github.com/bamboo120/airbnb-data-analysis/blob/main/Seattle_beds.png "Seattle Airbnb beds")![alt text](https://github.com/bamboo120/airbnb-data-analysis/blob/main/Boston_beds.png)

Up one: Seattle beds histogram Down one: Boston beds histogram

The number of beds here is used to study the size of people like booking. The common size of a place with beds is around 1 or 2. The average number of beds the host provided is 1.6 in Boston, and 1.7 in Seattle. 

 ### most polular price for the host place
![alt text](https://github.com/bamboo120/airbnb-data-analysis/blob/main/seattle_price.png "Seattle Airbnb beds")![alt text](https://github.com/bamboo120/airbnb-data-analysis/blob/main/boston_price.png)

Up one: Seattle price histogram Down one: Boston price histogram

From the histogram from Boston and Seattle, it seems that the most popular price is around $100. And the average price in Boston is $198, and $138 in Seattle. 


### features affect the review score rating

![alt text](https://github.com/bamboo120/airbnb-data-analysis/blob/main/cor.png)

Boston Airbnb correlation map

The plot above only show the numerical feathers to affect the rating score. The features with larger absolute value means it affects the review score more. From the image above, we can see that the happiness of your guest does not depend on the size of your room, it depends on the cleanliness, the accuracy of your description, the checkin, the way you communication, and the location.

![alt text](https://github.com/bamboo120/airbnb-data-analysis/blob/main/seattle_feather.png "Seattle Airbnb beds")![alt text](https://github.com/bamboo120/airbnb-data-analysis/blob/main/boston_feather.png)

## Summary the Results

1: The popular size are 1-2 beds for host

2: The popular price is around $100

3: The top features affects the review score rating are:

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

The code top10feather.ipynb is aim to test the top 10 features affect the review score.

## python library

numpy

pandas

matplotlib.pyplot

sklearn

seaborn

## acknowledgments

This is Udacity data science nano degree project. The data is from kaggle [Boston Pages](https://www.kaggle.com/airbnb/seattle/data) [Seattle Pages](https://www.kaggle.com/airbnb/boston)
