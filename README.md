# Movies_ETL

## Summary
For this challenge we are creating an automated pipeline that takes in new data , performs the appropriate transformations, and loads the data into existing tables.
We are refactoring code to create one function that takes in three files -Wikipedia data, Kaggle metadata, and the MovieLens rating data - and performs the ETL process by adding data to a PostgreSGL database.

### Resources 
- Data Source: movies_metadata.csv, ratings.csv, wikipedia-movies.json
- Python 3.8.8, Jupyter Notebook, PostgreSQL 11.13, pgAdmin 4

## Results
First we wrote and ETL function to read the three files and convert them to Pandas dataframes. The next process was to extract and transform all of the  data so it could be cleaned and merged into one dataframe, movies_with_ratings_df. Lastly the data was added to a PostgreSQL database with two tables, movies and ratings.  

After the code was refactored we were able to create a streamlined process to clean, merge and export the data into two databases.
The first table created, movies, resulted in 6,052 rows.

<img width="553" alt="movies_query" src="https://user-images.githubusercontent.com/89098766/139540919-ee14a6a7-9113-44f7-9ca3-5de74e5fe3d1.png">

The second table created, ratings, resulted in 24,024,289 rows.

<img width="413" alt="ratings_query" src="https://user-images.githubusercontent.com/89098766/139540946-5a784102-2374-419a-86d4-dfa722eff5db.png">
