# A closer look at New York and Toronto AirBnB data
This project analyzes AirBnB listing, calendar and review data for New York and Toronto (retrieved from [InsideAirBnB](http://insideairbnb.com/get-the-data.html) on September 10th 2020). It compares prices, reviews, availability for the two cities and selected neighbourhoods and includes a word analysis of reviews and listing names. 

## Table of Contents
1. [Installations](#installations)
2. [Project Motivation](#motivation)
3. [File Overview](#overview)
4. [Key Results](#results)
5. [Acknowledgements](#acknowledgements)

## <a id="installations"/> Installations

This project used Python 3 within Jupyter Notebook, plus the following libraries: 
- pandas
- NumPy
- matplotlib and seaborn
- re
- nltk
- itertools
- collections

## <a id="motivation"/> Project Motivation
The motivation of this project was to practice communicating data insights by:
- Deciding on a dataset to analyze and questions about the dataset to find answers to and communicate
- Gaining business and data understanding
- Preparing the data by performing necessary cleaning and data wrangling
- Perform analyses and evaluate the results
- Share the insights with stakeholders

The questions posed during analysis were: 
1. When is the best time to visit New York and Toronto?
     What are the busiest times of the year to visit New York and Toronto? By how much do prices spike?
2. What budget do I need to plan for accomodation in both cities?
     What does an AirBnB stay in New York and Toronto cost (on average, minimum, maximum)?
3.  In which neighborhoods should I stay?
     Which are the neighbourhoods with the highest density of Airbnb accommodations?
     Which neighbourhoods have the best average reviews? How do they compare on location review score?
     How do the neighborhoods compare in price?
     How do the neighbourhoods compare in availability of certain room types?
4. Do different neighbourhoods have a different vibe?
     What are the most common words used to describe a listing?
     How does this compare from New York to Toronto  and for different neighbourhoods? 
     Are the same words used in the review texts?

##  <a id="overview"/> File Overview
Included in the repository:
- Great Places to Stay: A closer look at New York and Toronto AirBnB data.ipynb: Jupyter Notebook with the project code
- newyork_data/map_ny.png: map of New York, source: [OpenStreetMap](https://www.openstreetmap.org/)
- toronto_data/map_to.png: map of Toronto, source: [OpenStreetMap](https://www.openstreetmap.org/)

Not included in the repository: 
- newyork_data/listings.csv: detailed listings data for NY
- newyork_data/reviews.csv: detailed review data for listings in NY
- newyork_data/calendar.csv: detailed calendar data for listings in NY
- toronto_data/listings.csv: detailed listings data for Toronto
- toronto_data/reviews.csv: detailed review data for listings in Toronto
- toronto_data/calendar.csv: detailed calendar data for listings in Toronto

The above files were all retrieved from [InsideAirBnB](http://insideairbnb.com/get-the-data.html) on September 10th 2020. 

## <a id="results"/> Key Results 

Find an overview of key findings on [Medium](https://medium.com/@maren.zoller/great-places-to-stay-a-closer-look-at-new-york-and-toronto-airbnb-data-71d8d134a6cf).

## <a id="acknowledgements"/> Licenses and acknowledgements

For the data, I must give credit to both AirBnB and InsideAirBnB. The data is available under a Creative Commons CC0 1.0 Universal (CC0 1.0) "Public Domain Dedication" license, more info can be found [here](http://insideairbnb.com/get-the-data.html).
