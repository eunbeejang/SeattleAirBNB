# Udacity Data Scientist Nanodegree
## Project: Writing a Data Scientist Blog Post

### Table of Contents

1. [Installation](#Installation)
2. [Project Motivation](#Project-Motivation)
3. [Data](#Data)
4. [File Descriptions](#File-Descriptions)
5. [Result](#Result)
6. [Blog](#Blog)

### Installation

This project requires **Python 3.x** and the following Python libraries installed:

- [SciPy](https://www.scipy.org/)
- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [seaborn](https://seaborn.pydata.org/)
- [scikit-learn](http://scikit-learn.org/stable/)


You will also need to have software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html)

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.

### Project Motivation

> For this project, I'm interested in answering following questions about Seattle AirBNB Listings.

1) What types of listings are popular?
2) When is the best time of the year to start a marketing campagn?
3) How well can we predict the price of a listing? What aspects correlate well to listing prices?

### Data
The data used for the project is Seattle AirBNB Dataset and it can be downloaded from **Kaggle**:

[Seattle Airbnb Open Data](https://www.kaggle.com/airbnb/seattle/data)


### File Descriptions

Jupyter Notebook ([seattleairbnb.ipynb](https://github.com/eunbeejang/SeattleAirBNB/blob/main/seattleairbnb.ipynb)) works related to the above questions. 


### Result
- According to my analysis, the popularity of a listing is defined by type and the location of the property. The trend differs by the room_type (ie. entire place, private room, and shared room). For listings with ehtire place, most popular listings were Bed&Breakfast, Cabin, and Camper/RV located in Rainier Valley, Queen Anne, Northgate, and Ballard. For listings with private rooms, Bed&Breakfast, Cabin in Downtown and Queen Anne were popular. For shared units, apartments in University District was the most popular listing type.

- The overall trend shows declining occupancy rates throughout the year 2016. This means that AirBNB renting activity in Seattle is decreasing. However, surge of rental activities are observed between April and August 2016 and there is another spike in renting activities in January 2017, which could be contributed by the end-of-the-year holiday season. If Seattle AirBNB marketing team is to start a campaign, they should aim for users booking for summer vacation or near the end of the year.

- For modelling the price of listings, I utilized data columns related to the accommodation details without any host-written descriptions or image of the property. Using a linear regression model, the rsquared score for training data was 56% and 52% for testing data. This shows that the model is hard to generalize the pricing of listing properties using the data columns provided. However, when analyzed the coefficients, property type and location(neighbourhood) appears to be the main factors for pricing for given data.

### Blog

