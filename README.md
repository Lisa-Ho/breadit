# About this project

This is a personal project scraping and analysing data from the []Reddit/Sourdough](https://www.reddit.com/r/Sourdough/) community in 2020. 

As a sourdough baker myself, I wanted to explore lockdown baking trends in more detail, see when engagement peaked and what bakers were talking about. 

Thanks to [pushshift.io](https://pushshift.io/api-parameters/) I was able to retrieve data from Reddit relatively easily. 

The write up of my analysis can be found on [my blog](https://inside-numbers.com/blog).

## Notebooks

This project is organised in two different jupyter notebooks.

1. Webscraping (data collection)
2. Data cleaning and analysis

## Requirements

This project is run on python 3 and a number of python libraries specified in ```requirements.txt```.

## Notes on methodology

### Users

Users are those who posted a submission in r/Sourdough in 2020. Some users have since then been deleted and are counted as one single [deleted] user. 

### Score / upvoting data

Unfortunately, the data retrieved through pushshift for submission scores (upvotes) seemed to be incorrect, so could not be used for analysis. 

### Dates and times

When converting unix timestamp to datetime, I did not account for different timezones of users at the time of their submission. Hence, analysis of submissions by days and hours of the day might be slightly distorted. 
