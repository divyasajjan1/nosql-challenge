# nosql-challenge
No SQL Mongo DB Challenge

Part 1: Database and Jupyter Notebook Set Up [NoSQL_setup_starter.ipynb](C:\Users\divya\Documents\nosql-challenge\NoSQL_setup_starter.ipynb)

1. Imported the data provided in the establishments.json file from the Terminal. 
    mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json

2. Imported the required libraries - Pymongo, pandas and pprint.
3. Created an instance of mongo client.
4. Created a database and verified that all the data has been loaded properly.
5. Assigned the establishments collection to a variable.

Part 2: Update the Database [NoSQL_setup_starter.ipynb](C:\Users\divya\Documents\nosql-challenge\NoSQL_setup_starter.ipynb)

1. Added a new restaurant to the 'establishments' collection.
2. Found the BusinessTypeID for "Restaurant/Cafe/Canteen" and updated the new restaurant with the BusinessTypeID found.
3. Deleted the records containing Local Authority as 'Dover'. 994 rows were deleted.
4. Updated the datatype of 'latitude' and 'longitude' from string to decimal, and 'RatingValue' from string to integer.

Part 3: Exploratory Analysis [NoSQL_analysis_starter.ipynb](C:\Users\divya\Documents\nosql-challenge\NoSQL_analysis_starter.ipynb)

Answered the following questions:

1. Which establishments have a hygiene score equal to 20?
    - Number of documents: 41
2. Which establishments in London have a RatingValue greater than or equal to 4?
    - Number of documents: 33
3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, 
    "Penang  Flavours"?
    - Got the top 5 results.
4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out
   the top ten local authority areas.
   - Using aggregation method, found the top 10 results of hygiene score 0 local areas.