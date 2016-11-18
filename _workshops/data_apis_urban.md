---
layout: workshop
sort_order: 15
title: "Data APIs in Python to Improve Urban Life"
image: "socrata_open_data.png"
repo: "https://github.com/dsiufl/DataAPIs-Workshop"
summary: > 
  Introduction to using data APIs from Python and publicly availible data from the 
  <a href="https://data.cityofgainesville.org/">City of Gainesville</a>.

---
Data science doesn't work without data! Getting access to and formatting data often the most difficult and time comsuming
part of an analysis. Open APIs make data access simpler and faster and understanding how they work will make a world of
data availible to you.

This workshop uses Python to explore a range of typical data APIs. The focus will be on visualizing urban data including 
poverty metrics from the US Census and utility usage data from the City of Gainesville's open data portal.


## Software Configuration

For this workshop we will be starting with the same software at in the 
[Python0](/workshops/python_0/)
workshop so please review the set up instructions there to get Anaconda and 
Jupyter notebooks running on your machine.

### Additional Packages

You will also need some additional Python packages. More details about how to 
install these in Anaconda are coming.
    
1. census
1. basemap
1. geocoder

### API Keys

Some APIs require API keys (a text string that is issued to you so they can 
monitor and restrict your usage) which you will need to also obtain before the 
workshop.

You will need to visit these links to get an API key for the US Census data and
for the Google mapping API. Both are free.
    
1. [US Census API key request](http://api.census.gov/data/key_signup.html)
1. [Google Mapping API key request](https://developers.google.com/maps/documentation/geocoding/get-api-key#get-an-api-key)
   You should be able to just click the "GET A KEY" button, you don't need to do the 6-step process.
   
### The Python notebook

The notebook for the workshop will soon be availible on Github.