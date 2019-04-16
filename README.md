# AirBnB Seattle and Boston Data Analysis

This repository contains a Jupyter notebook containing analysis that I completed on the Kaggle/AirBnb Boston/Seattle datasets as part of the Udacity Data Scientist Nanodegree. It also includes the data files I used in the analysis.

## Installations 
Libraries used in the data analysis include [pandas](https://pandas.pydata.org/), [numpy](http://www.numpy.org/), [seaborn](https://seaborn.pydata.org/), [matplotlib/pyplot](https://matplotlib.org/api/pyplot_api.html), and [scikit-learn](https://scikit-learn.org/stable/). These are all super well-known Python libraries, and further installation instructions can be found on their respective websites (linked).

## Motivation
The primary motivation for this project was to complete a component of the Udacity Data Scientist Nanodegree. I chose to explore the AirBnb Boston and Seattle datasets and answer the following business/data questions:

#### 1. How does listing availability and price change over the course of the year?

*Why does this matter?* Understanding listing availability and price patterns helps us understand how different markets compare to each other. We could potentially take an understanding of when listing availability is high or low in a particular and run a specific promotion in order to attract attention to this particular market. 

#### 2. How do the number of reviews fluctuate over the course of the year? What are the most common reviewer names? What are the most common words in reviews?

*Why does this matter?* Understanding how the number of reviews fluctuate over the course of the year can give us information on how users are interacting with the platform. Monitoring data also helps you catch when number of reviews are decreasing at an undesirable rate, and figure out how to address the problem if necessary. Common reviewer names is more of a fun tidbit, but could be used to create some fun marketing campaigns. The most common words in reviews can also help us learn what reviewers care most about in different markets, which can then be used to make business decisions as well. 

#### 3. What are some of the features most correlated with price?

*Why does this matter?* Understanding features most correlated with price help you better understand what's most or least valuable in each market. It doesn't necessarily tell you what consumers or suppliers themselves find most valuable, but one tangible way this information can be used is to enable you to give suggestions to landlords on how to price their listing, for example, or suggest the best deals (relative to other listings) for consumers.

## File descriptions
- data/boston-airbnb-open-data
  - calendar.csv, listings.csv, reviews.csv - These are the three Boston data files used in the analysis, which include information on Boston AirBnB listings, reviews, and calendar/availability.
- data/seattle
  - calendar.csv, listings.csv, reviews.csv - These are the three Seattle data files used in the analysis, which include information on Boston AirBnB listings, reviews, and calendar/availability.
- airbnb_seattle_boston_data_analysis.ipynb - This is the Jupyter notebook containing my analysis.

## Summary of results
Read the notebook for the results! Just kidding. Here's a quick summary to what I found for each question:

1. **Availability:** Seattle availability started at ~45% in Jan 2016 and climbed sharply until April, where it dropped from 75% to 65%, then remained relatively steady until dropping again in July to 60%, and then climbing through the rest of the year to peak at 75% in Jan 2017. Boston availability starts a bit lower, at ~25% in September, climbing sharply to *peak* at around 60% in Jan 2017, and then stay around ~55% until March, at which it drops again and stays steady at around ~50% until Sep 2017.

- **Price:** Prices for Seattle peak in the summer, while prices for Boston seem to peak in September from this dataset, with one unusual price spike in April, which may correspond to something like spring break Or... the Boston Marathon! That makes a lot more sense. The Boston Marathon is a pretty huge event, so it's intuitive that it would definitely impact price and availability dramatically.

2. **Number of reviews/month:** People tend to write the most reviews in the summer, and the number of reviews has been increasing steadily since 2009. Volume of reviews writtn for Seattle is slightly higher than Boston.

- **Most common reviewer names:** The most common male reviewer name is David for both Seattle and Boston; Sarah is the most common female reviewer name as well. My own name, Brian, ranks 14 in Seattle and in the 20s for Boston.

- **Most common words used in reviews:** 
  - Common words used in reviews for both cities *great, stay, place, clean, comfortable, location* 
  - Words used proportionally more common in Seattle reviews: *view, hill, downtown, bus, light, bars, fun, space, coffee, stocked* 
  - Words used proportionally more common in Boston reviews: *station, airport, floor, fine, old, rooms, public, apartment, air*

3. **Top predictors (by coefficient magnitude) of listing price**
- Seattle: 
  - Positive features: host verified by sent ID, wireless Internet, doorman, and # of bedrooms and bathrooms
  - Negative features: room type - shared, room type - private
- Boston:
  - Positive features: super strict 30-day cancellation policy, host verified by phone, doorman, # of bedrooms
  - Negative features: host verified by sent ID, room type - private
## Authors
The author of the notebook is me! Data provided by Kaggle and AirBnb, linked below in the acknowledgements.

## Acknowledgements
Thanks to Kaggle and AirBnB for providing the [Boston](https://www.kaggle.com/airbnb/boston) and [Seattle](https://www.kaggle.com/airbnb/seattle) data I used in this analysis. Thanks to Udacity as well for including this project as a part of their Data Scientist Nanodegree. I got some cool experience with writing my first Github readme in particular, hehe.

