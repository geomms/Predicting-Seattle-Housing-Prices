README Mod 2 King Country Housing Price

# King County, Seattle, Washington ,  USA 
### Project Details:
### Presentation URL: https://www.canva.com/design/DAD3vtuuMy8/O5Ilu5Rdr0DjdZMn9xxaEw/view?utm_content=DAD3vtuuMy8&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink
#### Goals  
- Find the price range of the majority of the houses.
  - Compare house sizes and prices per zip code.
  - Create price prediction model.
  - Prediction model.
  - Find the price range of the majority of the houses.

- Data used: King County dataset, years 2014-2015.
- Metric: average prediction within +/-$56,232.
- Average Price: ~$490,000
- Median Price: $440,000
- Prices Range: less then $1.3 mln 
  - 96% of the data was below $1.3 million

#### Business Problems:
- What area is in my price range? What area has the best price per sqft?
- What is the average price for that zip code?
- Where are alternative areas with the same house features but more affordable price?
#### Solutions:
- Removing data above $1.3 million (Crazy outliers above $1.3 mill)
- Selecting the right features and checking score results of models.
#### Recommendations for further developments:
- More recent data for current estimate.
- Predictions for how houses will appreciate or depreciate in value over time.
- Improve model.

## Project Intro/Objective
  We displayed house sizes, prices per zip code, price per sqft, price ranges, and home features with data visuals.
  Having visuals allowed us to identify the price differences for zip codes.
  With the data what was given to us, we also created a price prediction model. We trained and tested our model to predict      future prices given the features that the model has trained on. 
  Some of the features that we used were 
  - 'price'
  - 'bedrooms'
  - 'bathrooms'
  - 'sqft_living'
  - 'sqft_lot'
  - 'floors'
  - 'grade'
  - 'sqft_above'
  - 'sqft_basement'
  - 'zipcode'
  - 'lat'
  - 'long'
  - 'sqft_living15'
  - 'sqft_lot15'
  
## Project Findings:
- Features such as 'id', 'date', 'waterfront', 'view', 'condition', 'yr_built', and 'yr_renovated' did not help too much on predicting price.
- From our data visuals, zip code seem to play a big factor on prices. 
- From the Decision Tree Regressor the MAE increased after transforming and scaling features. (Possibly overfitting)
- From Random Forest the MAE also increased after transforming and scaling features. (Possibly overfitting)
- Both Decision Tree and Random Forest R2 score did improve by ~ 2-5%.


### Methods Used
* Statistics
* Data Cleaning
* Data Organizing/Exploring
* Feature Engineering
* Machine Learning
* Data Visualization
* Predictive Modeling
* Log Transformation
* Min-Max Scaling

### Metrics Used:
- Mean Absolute Error: we wanted to see the + and - in dollars that the models predicted.
- R2 score: we wanted an indicator that would tell use the accuracy % our models are performing. 
- 

## Models Used:

### Decision Tree Regressor (Anh)
  - Decision Tree did not do so well at predicting future unknown data. (Weakness: May be overfitting)
  - The initial score mean absolute error & R2 
    - MAE Score: 103564.73759259259
    - R2 Score: 0.6560417913775461
  - After finding best leaf_nodes to use:
    - MAE Score: 92981.27526326235
    - R2 Score: 0.6954556318824348
  - After Feature Engineering: (Some minor imporvements on the model here. MAE did go up from the last test, but R2 score improved)
    - MAE Score: 96855.61173606818
    - R2 Score: 0.7386150819288836
### Random Forest Regressor (Anh)
  - Random Forest did a decent predicition. (Weakness: Possible overfitting as well)
    - MAE Score: 73762.70740831373
    - R2 Score: 0.7950082670186805
  - After Feature Engineering:(Some minor imporvements on the model here. MAE didn't improve, while R2 did)
    - MAE Score: 75174.91694989661
    - R2 Score: 0.8137494114589178
    
    
### Technologies
* Python
* Pandas, Jupyter
* Seaborn
* Matplotlib
* Numpy
* Scikit learn


## Project Description
Since the data provided was 2014-2015, we did not have the most earliest data to train our model. Some of the hypothesis questions that we had was if location influenced price. Things such as longitute/ latitude or zipcode.
We created a map to input the data and saw that some zipcodes had a higher average price and some lower. 


## Needs of this project
- frontend/backend developers
- data exploration/descriptive statistics
- data processing/cleaning
- statistical modeling
- writeup/reporting
- real estate agents/companies
- housing price/sales
- house price predictions
- buyer and seller references


## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [here](Repo folder containing raw data) within this repo.

    *If using offline data mention that and how they may obtain the data from the froup)*
    
3. Data processing/transformation scripts are being kept [here](Repo folder containing data processing scripts/notebooks)
4. etc...

*If your project is well underway and setup is fairly complicated (ie. requires installation of many packages) create another "setup.md" file and link to it here*  

5. Follow setup [instructions](Link to file)



#### Project Members:

|Name     |  Github   | 
|---------|-----------------|
|[Mark Subra](https://github.com/geomms)
|[Abzal Seitkaziyev](https://github.com/xs-abzal)
|[Anh Phan](https://github.com/anhbiphan)


