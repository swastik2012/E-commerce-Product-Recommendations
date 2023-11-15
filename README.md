# E-commerce-Product-Recommendations
**Overview:**

The provided code demonstrates the implementation of a simple collaborative filtering recommendation system using the Surprise library for a dataset consisting of product ratings. Additionally, there is an example of item-based recommendation using cosine similarity.

### Part 1: Collaborative Filtering with Surprise
1. **Dataset Creation:**
   - Two datasets are created, namely `product_data` and `ratings_data`, representing product information and user ratings, respectively.

2. **DataFrames:**
   - The datasets are converted into pandas DataFrames (`product_df` and `ratings_df`).

3. **User-Product Rating Matrix:**
   - A user-product rating matrix (`user_prod_ratings`) is created using the `pivot` function.

4. **Collaborative Filtering Model:**
   - The Surprise library is used to build a collaborative filtering recommendation model using the Singular Value Decomposition (SVD) algorithm.
  
5. **Model Evaluation:**
   - The model is trained and tested on the dataset, and the Root Mean Squared Error (RMSE) is calculated to evaluate its performance.

6. **Recommendation Function:**
   - A function, `get_recommendations`, is defined to provide top N recommendations for a given product based on ratings.

7. **Sample Recommendations:**
   - Recommendations are generated for a sample user and product, and the top recommendations are printed.

### Part 2: Item-Based Recommendation with Cosine Similarity
1. **Product Similarity Calculation:**
   - Cosine similarity is calculated based on product ratings, forming a product similarity matrix (`generes_similarity`).

2. **Recommendation Function:**
   - Another function, `get_prod_recommendations`, is defined to provide top N recommendations for a given product based on similarity.

3. **Sample Recommendations:**
   - Recommendations are generated for a sample product, and the top recommendations are printed.

### Part 3: Reading and Analyzing External Dataset
1. **Reading External Dataset:**
   - An external dataset (`data`) is read from a CSV file containing information about electronics products.

2. **Dataset Exploration:**
   - The structure and size of the dataset are examined, and missing values are checked.

### Part 4: Integration with Surprise for Collaborative Filtering on External Dataset
1. **Surprise Integration:**
   - The external dataset is converted into a Surprise-compatible format.

2. **Collaborative Filtering Model on External Dataset:**
   - The same collaborative filtering model is trained and evaluated on the external dataset, showcasing the flexibility of the Surprise library.

### Conclusion:
The code provides a comprehensive example of building collaborative filtering recommendation systems using both an in-built dataset and an external dataset. It demonstrates the versatility of the Surprise library for collaborative filtering tasks.
