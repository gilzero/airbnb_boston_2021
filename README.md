# Boston Airbnb Listing 2021

## Table of Contents
- Project Background
- Author
- Data Source
- Libraries Used
- Motivation for The Project
- Files
- Summary of the results
- Acknowledgment

---- 

### Project Background
This project is to analyze Airbnb listing data on Boston 2021. (Latest scraped data from Airbnb OpenData at the time of writing)

Oct 2021

---- 

### Author
Weiming Chen (Alan)

---- 

### Data Source
[http://insideairbnb.com/get-the-data.html][1]
[http://data.insideairbnb.com/united-states/ma/boston/2021-09-19/data/listings.csv.gz][2] (19 September, 2021)

---- 

### Libraries Used
- numpy
- pandas
- matplotlib
- sklearn
- (Python 3.9 / Jupyter Notebook)

---- 

### Motivation for The Project
The main goal is to build a Airbnb Listing Price Estimator model by implementing machine learning from Boston 2021 data to generate a LinearRegression model. 
Host, agency, or end user can use this model to estimate / predict  listing prices by inputing some independent variables. 
I also tried to find out what most recent amenities are listed in Boston listing that new host might considering for his/her new listing. And some others like: most demanded/popular districts; price ranges distribution.

---- 

### Files
- /files/Boston_airbnb_2021/listings.csv
- boston_airbnb_2021_refactor.ipynb_

---- 

### Summary of the results
The Boston Airbnb Price Estimator/Predictor model I built based on this dataset is able to achieve 0.62 R-squared for training score, and 0.6 r-squared score for test score. The model can explain at least 60% of the variabilities of the data, could be a barebone working model in real life. 

However, for more accountable on predictability (aiming for \>0.7), I might need to train on more Boston pass data and experiment different features selection combination. (The model used 3000 instances/rows after cleaning and hot-one encoded categorical variables) I might aim for 6000 working(cleaned) instances to train. 

Price range distribution on this dataset reveals that 
$60-80 most offering range;
Overall, $80 - 160 range are popular;
Higher standard $180-220 also quite common in Boston also; 
Listing offerings drop significantly  after \> $220. 
Listing price median is $141 which makes more sense than mean: $191 as it might be affected/stretched by outlier in the data ($10000.00 per night)

---- 

### Acknowledgment
- Code snippet used about the function of train test, coefficients from Udacity example. 
- Plot on price range distribution inspired by the book “Data Science from Scratch” - Visualization chapter. 
- Some helper solution founds on StackOverflow. 

[1]:	http://insideairbnb.com/get-the-data.html
[2]:	http://data.insideairbnb.com/united-states/ma/boston/2021-09-19/data/listings.csv.gz