# Movie Recommender System 

### Algorithm used for this project (Item CF):

* Item Collaborative Filtering Algorithm
* Based on the similarity between items calculated using people's ratings of those items
* More convincing than the User CF for there are way more users than movies, movies change less frequently than users, and people will be more convinced by their own historical data than the choice of others who said to share similar interests with them 

To implement this project, we first derive the user's rating matrix from raw data, then build the co-occurrence matrix between the movies, then normalized the co-occurrence matrix to make every row add up to one. Last, we multiply the co-occurrence matrix and the rating matrix to get the recommended result. If the score of a movie that the user has not watched is greater than a certain threshold (in this case, the user's average rating) , we add it to the recommendation list. 
