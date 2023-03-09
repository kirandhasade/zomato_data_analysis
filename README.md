## Project Name: Zomato Data Analysis

## Project Objective:
Using Zomato dataset we try to find out following questions answer:
   1. Top 3 countries that uses the zomato?
   2. The country names that has given 0 rating?
   3. Which currency is used by which country?
   4. Which countries do have online Delivery options?
   5. List countries which have or have not online delivery options?
   6. Created a pie chart for top 5 cities distribution?
   7. Find the top 10 Cuisines?
   
## Analysis Involve Phases:
1. Data collection
2. Data Cleaning & Preparation
3. Data Analysis

## Phase 1: Data Collection
In this project, we are using 3 datasets:
1. Zomato dataset which include restaurant information along with its ratings details.
2. Country dataset that helps us to add country information from its country code from Zomato dataset.
3. Currency Exchange data from local currencies to US dollars.

## Phase 2: Data Understanding, Cleaning & Preparation
1. restaurant_id: 
- Unique id for each restaurant across various cities of the world
- Also this column is Primary key column in table. (Total number of rows in dataset: 9551 and total unique restarant ids are 9551.)

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
- As this columns doesn't effect other column values hence we are keeping as it's.

## Phase 3: Data Analysis

### Q1. Top 3 countries that uses the zomato?
- Maximum number of transctions is in India
- Zomato maximum records are from India followed by USA and united Kingdom

![Screenshot%202023-03-07%20at%2023.03.01.png](attachment:Screenshot%202023-03-07%20at%2023.03.01.png)

### Q2. 
