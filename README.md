# anime-recommendation-system
Overview 🌟📚
Welcome to the Anime Recommendation System! This project aims to provide personalized anime recommendations based on collaborative filtering techniques.

The application utilizes user-based collaborative filtering to find similar users based on their anime preferences and recommends animes liked by similar users that the target user has not watched yet. Additionally, the system employs item-based collaborative filtering to find similar animes based on their features (e.g., genres, synopsis) and recommends animes similar to the one provided by the user.

The dataset used for training and recommendation includes various anime titles, user ratings, and anime features such as genres and synopses. The model was trained using TensorFlow and Keras to create anime embeddings for both users and animes, facilitating efficient similarity comparisons.

Feel free to explore and enjoy the exciting world of anime recommendations with our innovative system!

collaborative filtering using K-Nearest Neighbors (KNN):

1. **Data Preprocessing**: Load datasets and perform necessary data scaling. Encode user and anime IDs to prepare data for model training.

2. **Model Architecture**: Implement a KNN-based collaborative filtering model. Instead of embeddings, KNN relies on calculating similarities between users or items based on their ratings or preferences.

3. **Model Training**: Train the KNN model using the dataset. This involves computing similarities between users or items and identifying nearest neighbors.

4. **Recommendation Generation**: Utilize the trained KNN model to generate recommendations. Similar animes or users are identified based on their proximity in the feature space, allowing for personalized recommendations.

Content-Based Filtering

The second part of this notebook explores content-based filtering, an alternate recommendation technique. Content-based filtering suggests animes to users based on attributes such as genres and ratings. Here, my key steps were:

TF-IDF Vectorization: I created a TF-IDF matrix for anime genres to quantify the importance of genres in each anime's description.
Cosine Similarity: By computing cosine similarity between animes based on their genre descriptions, we can determine their similarity.
Content-Based Recommendation: Leveraging the computed similarity scores and ratings, we now can recommend animes that are similar to a given anime, considering their genre and score.
We've got an exciting mix of collaborative and content-based filtering models, ensuring we can deliver diverse and accurate anime recommendations tailored to the preferences of each user. 🤗
