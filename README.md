# imdb_bollywood_movie_scrap_analysis

Objective
Bollywood has witnessed exponential growth in terms of volume of business, manpower employed, the number of movies produced each year and also the global reach. There are a number of factors like Actors, Directors, Time of Release, Genre, Production house, etc. which affect the outcome of a movie. This Dataset contains movie title, release date, genre, writers, directors, sequel and hit/flop count of various movies. Bollywood Actors and Actress ranking dataset is also used for their overall rating and performance based on google hits and likes.

Existing System
Previously, different predictions on dataset like whether the movie will be hit or flop has been given. And the movie recommendation system for users has been made for their preferred taste of movies. Twitter reactions for the upcoming movies and after watching it, based on the majority votes success of the movie can be predicted. User is also suggested a movie which they will prefer to watch based on their past watch history.

Need for the Project	
We are going to perform a new type of prediction on dataset based on clustering different categories of actors and directors by their preferred movie types. This will help to determine the coordination between actor and director. It will also predict the movie type mostly chosen by an actor. Example: Akshay Kumar always prefers that movies which are related to social causes and inspires the young generation. Based on the movie type and different categories like genre and writer, we will make a further prediction that the actor will choose that movie to work or not.
We are also going to analyse different movie actors and directors ranking based on their movie counts and success ratios.	
DESIGN AND IMPLEMENTATION DETAILS
This section describes how dataset is generated and complete visualisation on our dataset.
1.	There are 800 instances (movies) in total. Our dataset contains all possible instances from the webpage. For each instance, it consists of certificate, duration, rating, genre, vote, gross. We used Imdb url: https://www.imdb.com/list/ls005197923/?st_dt=&mode=detail&page='+str(x+1)+'&sort=list_order,asc  to scrap data. Initially, we got data that contained lots of NULL values and raw formatted data.
 
2.	 Cleaning of Data:
Initially, we drop the Movie Title column which was not required in our dataset and the Genre column contained ‘\r\n’ at the beginning, therefore we cleaned the dataset.
 
3.	After cleaning, Final dataset looked like:
 

We need to study director and actor top ratings based on Genre Type. With the help of the Pandas dataframe, we analyzed that.
Group by method was used to group directors based on Genre type.








4.	Top directors and their rating:
  
Top stars and their Rating on different Genre type:
 




                                                        4
                                                 RESULT
Top stars and their rating for action:
 
Director Actor Coordination:
 




Mostly preferred actor for a particular director.
 
 
