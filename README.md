# PennAppsXX
## Clustering Movie Scripts into Subgenres To Improve Recommendation Systems
Movies are often categorized into broad genres, such as horror, drama, and comedy. However, this does not reflect the diversity within these genres.
We wanted to see if there were other features (that could be automated#) that would improve recommendation systems.
We chose to analyze scripts because of their accessibility, and our knowledge of NLP embeddings.

## Datasets
* MovieLens - the MovieLens dataset is a well-studied dataset for recommendation systems. Users explicitly rate movies.
* IMSDB - we scraped the scripts from IMSDB.com. This is a smaller subset of movies, but it was the most accessible.
* FastText - used for word embeddings.

## Models
* Gaussian Mixture Model - Discerns components given categories. k=3 components. Full covariance matrix. Default initialization.
* Item-based Recommendation System - Recommends items based on similar items. Cosine similarity. We created recommendation systems using 1) ratings, 2) ratings, genres, 3) ratings, genres, subgenres.

## Challenges encountered
* Finding a good enough dataset
* Finding a good embedding

## Potential improvements
* Increasing diversity of scripts
* Further tuning initialization, covariance matrix, iterations
* Overfitting using regularization
* Similarity metric using Pearson, adjusted cosine
* Grid search for ideal N-components to split genres into and for similarity value multipliers (when genres and/or subgenres of two movies match).
