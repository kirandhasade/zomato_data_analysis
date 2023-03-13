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
3. Created a dictionary for currency exchange in dollars for analysis
  
## Phase 2. Data Understanding, Cleaning & Preparation

### Observation: 
1. restaurant_id: 
- Unique id for each restaurant across various cities of the world
- Also this column is Primary key column in table. (Total number of rows in dataset: 9551 and total unique restarant ids are 9551.)
- <img src=graphs_screenshots/Q.1_screenshot.png>

2. restaurant_name:
- Restaurant name belongs to its id.

3. country_code:
- Code for each country.
- Country in which restaurant is located
- There are total 15 unique country codes in this dataset.

4. city:
- City in which restaurants are located.
- There are total 141 cities restaurant data into the dataset.

4. address:
- Address of restaurants.

5. locality
- Locality of restaurants in that city.
- There are total 1208 unique localities data into the dataset.

6. locality_verbose
- Represents detailed description of the locality
- We can drop  either 'locality' or 'locality_verbose' columns as it contains similar information.
 
7. longitude
- Represents geographical longitude coordinate of the restaurant’s location.

8. latitude
- Represents geographical latitude coordinate of the restaurant’s location.

9. cuisines
- Represents different types of Cusines offered by the restaurants.
- There are total 1825 unique cuisines.
- There are total 9 null values in cuisines, means restaurant cusinies information is not available.

10. average_cost_for_two
- Represents average cost for 2 persons in local currency.

11. currency
- Represents Currency of every country
- There are 12 unique currency

12. has_table_booking
- Represents whether the restaurant has table booking or not.
- It is boolean datatype 

13. has_online_delivery
- Represents whether the restaurent has online delivery option or not.
- It is boolean datatype

14. is_delivering_now
- Represents whether the restaurent will be able to deliver at specific timing.
- It is boolean datatype

15. switch_to_order_menu
- It is boolean data type
- It has 9551 No records
- We can drop this column as it doesn't contain any informative information in further analysis.

16. price_range
- represents range of price of food.
- There are total 4 unique values in price range.
- It is a array which contains [1,2,3,4].

17. aggregate_rating
- Represents rating of restaurant out of 5.
- There are toatal 33 unique values in aggregate_rating.
 
18. rating_color
- There are total 6 unique rating colour with respect to aggregate rating column.
- Represents colour to specific range  with reference to aggregate_rating column.

19. rating_text
- there are total 6 unique rating text with respect to aggregate rating column.
- represents rating text of restaurant

20. votes 
- Represents number of ratings given to specific restaurant.

21. country
- Represents country of restaurant.
- There are total 15 unique countries in the dataset.

### Observation:
- Data is almost clean.
- We have 9 null values into Cuisines columns.
- As this columns doesn't effect other column values hence we are keeping as it is.


## Phase 3. Data Analysis

#### Q.1: Top 3 countries that uses the zomato?(SS)
- Maximum number of transctions is in India
- Zomato dataset maximum records are from India followed by USA and United Kingdom.

 #### Q.2 Find maximum number of rating?
When rating is between:
    - 4.5 to 4.9  ---> Excellent
    - 4.0 to 4.4  ---> Very good
    - 3.5 to 3.9  ---> Good
    - 2.5 to 3.4  ---> Average
    - 1.8 to 2.4  ---> Poor
- As labeled in graph - 3737 restaurants didn't have any rating.
- Rating shows normal distribution i.e. the data follows a bell shape, with most values clustering around a central region and tapering off as they go further away from the center.
- Maximum number restaurants are average rated i.e. between 3 to 3.5.

#### Q.3.Find the country names that have 0 rating restaurants.
- Maximum number 0 rated restaurants are from India i.e. 2139 restaurants.
- However only few restaurants are from other countries in which 5 are in Brazil, 3 in United States and 1 in United Kingdom.

#### Q.4 Distribution of restaurent across countries?
India has largest number of restaurants across countries which consit of 90% followed by United States and United Kingdom.

#### Q.5.  Find out which currency is used by which country?

#### Q.6. Which countries do have online Delivery options and which have not online delivery options?
Indian and UAE restaurants only have Online Delivery options in this dataset.

#### Q.7 Create a pie chart for  top 5 cities distribution.
New Delhi has maximum number of restaurants followed by Gurgoan and Noida

 #### Q.8. Find the top 10 Cuisines
- North Indian food dominates the Indian taste buds,because majority of the restaurents are based out of North India(Previosu graph).
- North Indian,Chinese,Fast food,Mughlai are few popular cuisines in India.

#### Q.9. Which country has cheapest food?
India has the cheapest average cost for 2 persons, followed by Sri Lanka and Indonesia.

#### Q.10 a) Create a tree map for cuisines for India
North Indian,Chinese,Fast food, Mughlai are few popular cuisines in India.

#### Q.10 b) Tree map for Cuisines for United States
- Americans love everything American- steak,seafood, burgers,BBQ apart from Mexican and Chinese food. 
- Popular Indian cuisine is North Indian owing to major North Indian cities and for the USA it’s all Americana food.

#### Q.11 a) Create a histogram for distribution of votes across India ?
A major of Indian restaurents ratings are Zero

#### Q.11 b) Create a histogram for distribution of votes across United States ?
- USA restaurants have higher ratings compared with Indian restaurants, this could indicate a better service in the US.
- US customers provide ratings more frequently and consistently than Indians.

### End Note
90% of observations belong to India.
                  
