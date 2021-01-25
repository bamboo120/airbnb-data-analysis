# airbnb-data-analysis


Business Understanding
1: Based on the data, what is the most polular size for the host place (like how many beds host are provided)?

2: Based on the data, what is the most popular price?

3: What feathers affect the review score rating?

Data Understanding

1: We can check the histogram and the mean value of beds.

2: We can check the histogram and the mean value of price.

3: I pick some related feathers affected the review score rating below: 'cancellation_policy','guests_included','host_response_time','host_response_rate','host_acceptance_rate','host_has_profile_pic','host_identity_verified','room_type','accommodates','bathrooms','bedrooms','beds','bed_type','price','number_of_reviews','review_scores_rating','instant_bookable','reviews_per_month','review_scores_value','review_scores_location','review_scores_communication','review_scores_checkin','review_scores_cleanliness','review_scores_accuracy'

Prepare Data

1: the data of beds is ready

2: the price need to change into float

3: except of review score rating, the int and float data NAN are replaced with the mean value. And dummy the categorical variables 

Data Modeling

Split training and testing data. Use 'review_scores_rating' as y, the rest feathers as X. Apply linear regression to learn the data.

Evaluate the Results



File description: 
All the data is in Archive.zip
In Archive.zip, boston.csv is the data of Airbnb price and data in Boston. seattle.csv is the data of Airbnb price and data in Seattle.
list_boston.csv is the feathers of airbnb in Boston. list_seattle.csv is the feathers of airbnb in Seattle. 

The code price1.ipynb is to calculate the price histogram and the beds histogram in Boston and seattle.
The code correlation.ipynb is to calculate the correlation of feathers.
The code top10feather.ipynb is aim to test the top 10 feather affect the review score.

python library

numpy

pandas

matplotlib.pyplot

sklearn

seaborn

acknowledgments

This is Udacity data science nano degree project. 
