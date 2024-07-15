# E-Commerce-Product-Recomendation-System
# Product-recommendation-e-commerce system
In order to offer users customized product recommendations based on their browsing and purchase history, I developed an e-commerce product recommendation system. This system analyzes user activity and generates recommendations using content-based filtering algorithms and collaborative filtering, which improves the shopping experience and increases revenue for e-commerce enterprises.


### Set of data
I assigned unique identities to an Amazon dataset of customer ratings for electronic devices in order to prevent biases. The Amazon Electronics Rating Dataset Recommendation is a dataset that can be downloaded [here](https://www.kaggle.com/datasets/vibivij/download?datasetVersionNumber=1).

### Methodology

1. **Rank-Based Product Recommendation** - **Objective**: Solve the Cold Start Problem and suggest the most well-liked products to prospective clients.
   - **Action**: Determine the overall number of ratings and the average rating for every product. Offer the best products with the required number of minimal interactions.
   - 
2. **Similarity-Based Collaborative Filtering**
   - **Objective**: Provide personalized recommendations based on similar users' interactions.
   - **Method**: Convert user IDs to integers, find similar users using cosine similarity, and recommend products that similar users interacted with but the actual user has not.

3. **Model-Based Collaborative Filtering**
   - **Objective**: Provide personalized recommendations using past behavior and preferences while addressing sparsity and scalability.
   - **Method**: Use SVD on a CSR matrix of product ratings to reduce dimensionality, predict ratings, and recommend top products based on predicted ratings.
   - **Evaluation**: Calculate RMSE to evaluate model performance by comparing actual and predicted ratings.
