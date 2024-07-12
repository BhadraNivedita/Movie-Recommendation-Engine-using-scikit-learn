# Recommentaion engine

Content-based and collaborative filtering are two primary approaches used in recommendation systems. Here are the key differences between them:

### Content-Based Recommendation Engine
## Principle: 
Content-based filtering recommends items similar to those that a user liked in the past based on the item's features.

#### How It Works:

##### Item Representation: 
Items are represented using their features. For example, a movie could be represented by its genre, director, cast, etc.
##### User Profile: 
A profile is created for each user based on the features of items the user has interacted with (e.g., liked, purchased, rated).
##### Similarity Measure: 
The system calculates the similarity between items based on their features and recommends items similar to those the user has liked in the past.

#### Advantages:

##### No Cold Start for Items: New items can be recommended as long as their features are known.
##### Personalized Recommendations: 

Tailored to individual user preferences based on item features.
#### Disadvantages:

##### Feature Engineering:
Requires detailed and high-quality features of items, which can be complex and resource-intensive.
##### Limited Discovery:
Users may not be exposed to items outside their existing preferences, leading to a narrow recommendation range (filter bubble).

[Example Jupyter notebook](https://github.com/BhadraNivedita/Movie-Recommendation-Engine-using-scikit-learn/blob/main/Content_based_Recommendation_system_movie_dataset.ipynb)

### Collaborative Filtering Recommendation Engine
Principle: Collaborative filtering recommends items based on the interactions and preferences of similar users.

#### How It Works:

##### User-Item Interactions: Utilizes user-item interaction data, such as ratings, purchases, or clicks.

##### Similarity Measure: Two main types:
###### User-Based Collaborative Filtering: 
Finds users similar to the target user and recommends items those similar users liked.
###### Item-Based Collaborative Filtering: 
Finds items similar to those the target user has interacted with and recommends those items.
##### Matrix Factorization: 
Techniques like Singular Value Decomposition (SVD) are used to factorize the user-item interaction matrix into lower dimensions for recommendations.

#### Advantages:

##### No Need for Item Features: 
Can work with only interaction data.
##### Serendipity: 
Can introduce users to items they might not have considered based on other users' preferences.
#### Disadvantages:

##### Cold Start for Users and Items: 
New users or items with no interaction history are hard to recommend accurately.
##### Sparsity:
In systems with many items and users, the user-item interaction matrix can be very sparse, making it difficult to find similarities.

[Example Jupyter notebook] (https://github.com/BhadraNivedita/Movie-Recommendation-Engine-using-scikit-learn/blob/main/Collaborative%20recommendation%20engine.ipynb)
