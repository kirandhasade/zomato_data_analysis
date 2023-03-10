## Project Name: Zomato Data Analysis

### Project Objective:
Using Zomato dataset we try to find out following questions answer:
   1. Top 3 countries that uses the zomato?
   2. Find maximum number of rating?
   3. Find the country names that have 0 rating restaurants.
   4. Distribution of restaurent across countries?
   5. Find out which currency is used by which country?
   6. Which countries do have online Delivery options and which have not online delivery options?
   7. Create a pie chart for  top 5 cities distribution.
   8. Find the top 10 Cuisines
   9. Which country has cheapest food?
   10.a. Create a tree map for cuisines for India. <br> b. Create a tree map for cuisines for United States.
   11. a) Create a histogram for distribution of votes across India ?<br> b) Create a histogram for distribution of votes across United States ?
### Analysis Involve Phases:
1. Data collection
2. Data Cleaning & Preparation
3. Data Analysis

## Phase 1. Data Collection
We are using two datasets:
1. Zomato dataset which include restaurant information along with its ratings details.
2. Country dataset that helps us to add country information from its country code from Zomato dataset.

# importing basic libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from matplotlib import rcParams
%matplotlib inline

# Zomato dataset
df=pd.read_csv('zomato.csv')
