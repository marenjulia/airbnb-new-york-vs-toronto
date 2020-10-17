README
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

**When is the best time to visit New York and Toronto?**

By popularity (proportion of booked listings and average listing price), Christmas time and the summer months are the best time to visit both cities. If one wants to optimize for lower prices and higher proportion of AirBnBs to choose from, autumn and winter (except December), are the best time to visit the two cities.

**What budget do I need to plan for accommodation in both cities?**

AirBnB listings in both cities cover a wide range of listing prices, including many high-priced outliers. My evaluation only featured available listings, and I evaluated median instead of mean listing prices. A night in a New York AirBnb has a 10 USD minimum, 112 USD median, and 13,798 USD maximum price. Therefore, the budget needed for a week (6 nights) is 60 USD minimum, 672 USD when assuming the median price, and maximum 82,788 USD. A night in a Toronto AirBnb has a 13 USD minimum, 100 USD median, and 13,00 USD maximum price. Therefore, the budget needed for a week (6 nights) is 78 USD minimum, 600 USD when assuming the median price, and maximum 78,000 USD.

**In which neighborhoods should I stay?**

Here, I reviewed all New York neighbourhood groups and the top 5 Toronto neighbourhoods with the highest AirBnB density. In New York most AirBnBs are in Manhattan, which has the best average location reviews, but also highest average prices and worst overall reviews. Staten Island has the best average reviews, second best location and a good price level. Brooklyn has the second most listings, second best review score and reasonable pricing level. Looking at the combination of reviews, price, location, and availability of Airbnb and room type options, Brooklyn and Staten Island seem to be the most interesting to what I am looking for. In Toronto, Waterfront Communities has the best reviews but also the matching prices. Combining all reviewed features, Annex can convince with a (comparably) reasonable price level, good reviews and okay location score average, while offering a wide range of room types to choose from.

**Do different neighbourhoods have a different vibe?**

In both cities, and across all evaluated neigbourhoods (Manhattan, Brooklyn, Staten Island, Waterfront Communities, Annex, and Niagara), basic description of room and apartment features dominate the listing names, e.g. "room", "bedroom", "apartment", "apt", "studio", "condo", or "suite". Adjectives that are used most common are "private", "cozy", and "spacious". New York listing names mention neighborhood names and listings being "sunny", Toronto listing names mention location ("downtown"), and transportation options ("parking", "subway"), and the attribute "home".

Manhattan listing names are focused on locations ("east", "west", "central" "park", "manhattan", "village"), Brooklyn listing names focus on being "sunny" and "beautiful", and mentions "loft" as another listing descriptor. Staten Island listings mention the "ferry", "private" is the most common listing descriptor. Waterfront listings mention "condo"s "downtown", the "cn" "tower", the "view", the "lake", "parking", "luxury" and are "modern". Annex listings are also mentioning "luxury", the "heart" of "Toronto" and locations like "yorkville". Niagara listings mention "parking", the "view", and the "lake" - and also "king" and "queen" (beds?).

Across both cities and neighbourhoods, reviewers praise "great", "place"s to "stay". Brooklyn and Manhattan review texts have similar most used words, with Brooklyn reviews using "clean" and "comfortable" more often. Again, Staten Island's unique selling point seems to be the "ferry". Waterfront listing reviews are "amazing" and have a "view". Annex review texts focus more on everything being "comfortable", "easy" and "close". Niagara reviews mention "amazing" and "easy", but not "comfortable" or a "view".
