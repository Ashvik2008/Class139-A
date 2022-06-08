#Class138

Data Collection : Data is used to create more efficient systems
Recommendation systems are a type of information filtering system as they improve the quality of search results and provide items that are more relevant to the searched item or are related to the search history

Amazon uses this to suggest products 

Youtube uses it to decide which video to plan next on autoplay 

Facebook uses it to recommend pages to like and people to follow

Companies like Netflix and Spotify depend highly n the effectivness of their recommendation engines for their business 


There are mainly three types of recommendation systems 

1) Demographic filtering (A particular sector of a population)
a-they offer generalized recomendations to every user, based on movie popularity
b-the system recommends the same movies to users with similar demographic features 
c-since each user is different this approach is considered to be to simple 
d- the basic idea behind this system is that movies which more popular and critically acclaimed will have a higher probability of being liked by the average audience

2) Content-based Filtering :
they suggest similar items based on a particular item.
the system uses item meta-data such as genre, director,description,actors etc or movies to make these recommendations
the general idea behind this recommendation system is that if a person likes a particular item he/she will also like an item that is similar to it 

3) Collaborative Filtering :
this system matches persons woth similar interests and provides recommendations based on this matching 
Collaborative filters do not require item meta-data like it's Content based couterparts

# Class139

Demographic Recommendation provides a general chart of recommended movies to all the users they are not sensitive to the interests of a particular user this is where a more refined system - content based filtering comes into play

Demographics plural : \ the statistical characteristics of human populations (such as age or income) used especially to identify markets a change in the state's demographics \ It is refered to a particulat of a poplation. In demographic filtering we want to offer generalised recomendation to every user. Step to find out top rated movies. We nee a metric or scroce to rate movie. We need to calculate the score for every movie. Finally we need to sort the score and recommend the best rated movis to user. Example:- A movie with 8.9 rated and 3 votes, Another movie with 7.8 rating and 40 votes. To calculate the best rated among those IMDB [internet movie database] has created a formula it is known as weighted rating and it is famousily used in the industry to get score for their product. Weighted Rating (WR) = ((v/v+m)R) + ((m/v+m)C) v - it is the number of votes for a particular movie \ m - is the number of votes required to be listed in the chat \ R - average rating of the movie \ C - mean votes across the who

IMDB

The Full form of IMDB is Internet Movie Database. IMDb is an online database of information related to movies, actors, directors, 
televisions shows, biographies, reviews, video games, plot summaries, and related information. The information stored on IMDb 
comes from different sources such as film studios, filmmakers, and other official sources.
-------------------------------------------

https://rahuls0959.github.io/ds-blog/python/recommendation%20system/relevancy/collaborative%20filtering/content-based%20filtering/demographic%20filtering/2020/06/06/_Recommendation-System_Part-1.html

-------------------------









https://www.kaggle.com/tmdb/tmdb-movie-metadata#
Kaggle link -|^

in this class we will be using the dataset from Kaggle
it contains the data for 5000 movies 

Refer Google Colab:
Login to kaggle 
Go to my accounts pages(Top right icon)
Go to API section -> Click on  create new API token 
Kaggle.json will get downloaded in your system 

● status - "Released" or "Rumored". 
● tagline - Movie's tagline. 
● title - Title of the movie. 
● vote_average - average ratings the movie received. 
● vote_count - the count of votes received.
Let’s understand the data. The first dataset contains the following features: 
● movie_id - A unique identifier for each movie.
 ● cast - The name of lead and supporting actors. 
 ● crew - The name of Director, Editor, Composer, Writer, etc.
The second dataset has the following features: 
● budget - The budget in which the movie was made. 
● genre - The genre of the movie, Action, Comedy, Thriller, etc. 
● homepage - A link to the homepage of the movie. 
● id - This is in fact the movie_id as in the first dataset. 
● keywords - The keywords or tags related to the movie. 
● original_language - The language in which the movie was made. 
● original_title - The title of the movie before translation or adaptation. 
● overview - A brief description of the movie. 
● popularity - A numeric quantity specifying the movie popularity. 
● production_companies - The production house of the movie. 
● production_countries - The country in which it was produced. 
● release_date - The date on which it was released. 
● revenue - The worldwide revenue generated by the movie. 
● runtime - The running time of the movie in minutes.
