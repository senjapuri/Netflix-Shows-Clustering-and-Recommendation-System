# Netflix Shows Clustering and Recommendation System

# Description
The Netflix Movies and TV Shows Clustering project involves exploratory data analysis (EDA) and clustering analysis on a dataset of Netflix content. The dataset includes movies and TV shows with attributes like director, cast, country, rating, genre, and description. The project aims to extract insights and patterns from the dataset, and cluster the content based on textual attributes to understand the categorization and trends.

# Objective
The objective of this project is to analyze the Netflix dataset to uncover patterns and trends in the content available on the platform. Additionally, the project aims to perform clustering to group similar movies and TV shows based on their attributes, providing a better understanding of the content distribution and characteristics.

# Attribute Information
- show_id : Unique ID for every Movie / Tv Show

- type : Identifier - A Movie or TV Show

- title : Title of the Movie / Tv Show

- director : Director of the Movie

- cast : Actors involved in the movie / show

- country : Country where the movie / show was produced

- date_added : Date it was added on Netflix

- release_year : Actual Releaseyear of the movie / show

- rating : TV Rating of the movie / show

- duration : Total Duration - in minutes or number of seasons

- listed_in : Genere

- description: The Summary description

# Conclusion
- *Key Findings from EDA*: Netflix hosts more movies than TV shows, with the total number of shows increasing significantly over time.The majority of shows were produced in the United States, catering predominantly to adult and young adult audiences.

- *Clustering Approach*: We decided to cluster the data based on attributes such as director, cast, country, genre, and description. These attributes were tokenized, preprocessed, and then vectorized using TFIDF vectorizer.

- *Feature Engineering*: Using TFIDF Vectorization, we generated 20,000 attributes.

- *Dimensionality Reduction*: Principal Component Analysis (PCA) was applied to reduce dimensionality. We found that 4,000 components captured over 80% of the variance, so we limited the components to 4,000.

- *Clustering Algorithms*: K-Means Clustering: Utilized the elbow method and Silhouette score analysis to determine an optimal number of 6 clusters. Agglomerative Clustering: Employed dendrogram visualization to identify 12 optimal clusters.

- *Content-Based Recommender System*: We developed a content-based recommender system using cosine similarity. This system provides 10 recommendations based on the type of show a user has watched.
