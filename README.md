# Netflix Recommendation System Using Python
 
The movie rating files contain over 100 million ratings from 480 thousand
randomly-chosen, anonymous Netflix customers over 17 thousand movie titles.  The
data were collected between October, 1998 and December, 2005 and reflect the
distribution of all ratings received during this period.  The ratings are on a
scale from 1 to 5 (integral) stars. To protect customer privacy, each customer
id has been replaced with a randomly-assigned id.  The date of each rating and
the title and year of release for each movie id are also provided.

TRAINING DATASET FILE DESCRIPTION
================================================================================

The file "training_set.tar" is a tar of a directory containing 17770 files, one
per movie.  The first line of each file contains the movie id followed by a
colon.  Each subsequent line in the file corresponds to a rating from a customer
and its date in the following format:

CustomerID,Rating,Date

- MovieIDs range from 1 to 17770 sequentially.
- CustomerIDs range from 1 to 2649429, with gaps. There are 480189 users.
- Ratings are on a five star (integral) scale from 1 to 5.
- Dates have the format YYYY-MM-DD.

MOVIES FILE DESCRIPTION
================================================================================

Movie information in "movie_titles.txt" is in the following format:

MovieID,YearOfRelease,Title

- MovieID do not correspond to actual Netflix movie ids or IMDB movie ids.
- YearOfRelease can range from 1890 to 2005 and may correspond to the release of
  corresponding DVD, not necessarily its theaterical release.
- Title is the Netflix movie title and may not correspond to 
  titles used on other sites.  Titles are in English.

  1. Analyse the data : check rating distribution

  2. Clean the Ratings dataset to have movie_id beside each ratings against customers

  3. Create a dataset with count and mean ratings for movie_ids, calculate  a benchmark by using quanlite, exclude movies with less that benchmark ratings.

  4. Create a dataset with count and mean ratings for cust_ids, calculate  a benchmark by using quanlite, exclude movies with less that benchmark ratings.

  5. Build the netflix recommendation System : First create a pivot table with columns as movie_ids, rows as cust_id and values as ratings.

  # find correlation with other movie titles using corrwith() and using PearsonR technique
    similar_to_target = df_p.corrwith(target,method='pearson')
    sort values descending order
    and send back the first 10

6. Calculate Manually as well

