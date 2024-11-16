# Movie-Recommendation-System

## Overview
This project is a content-based movie recommendation system using semantic embeddings generated with the Sentence Transformers library. It allows users to query for movies based on natural language descriptions, returning the most relevant recommendations. The system is designed to work with a dataset containing movie titles and genres.

## Features
### Content-Based Recommendations:
1. Uses natural language queries to recommend movies.
2. Provides relevant suggestions based on movie titles and genres.

## Embedding Representation:
1. Descriptions of movies are encoded into vector embeddings using a pre-trained transformer model (all-MiniLM-L6-v2).
2. Cosine similarity is used to match user queries with movie descriptions.
   
## Dynamic Query Support:
1. Handles a variety of user queries, such as:
2. Movies suitable for children.
3. Recommendations for specific genres like comedy or horror.
4. Suggestions based on release periods, e.g., 1990s romantic comedies.
   
## Dataset Description
### Source: movies.csv

## Columns:
- movieId: Unique identifier for each movie.
- title: Title of the movie with its release year.
- genres: Pipe-separated genres associated with each movie.

## Augmented Data:
- A new column, description, is created in the format:
- Title: {movie title}, Genre: {movie genres}.
- Example Queries and Recommendations
- Query: "Animated movie about bears that I can watch with kids"

## Recommendations:
- Care Bears Movie II: A New Generation (1986) – Animation|Children
- Brother Bear (2003) – Adventure|Animation|Children
- Query: "Movies falling under the comedy and horror genres"

## Recommendations:
- Hood of Horror (2006) – Comedy|Drama|Horror
- Detention of the Dead (2012) – Comedy|Horror
- Query: "Romantic comedies released in the 1990s"

## Recommendations:
1. Indian Summer (1993) – Comedy|Drama
2. Loins of Punjab Presents (2007) – Comedy
3. Tools and Technologies

## Libraries:
1. pandas: For data manipulation.
2. Sentence Transformers: For embedding generation.
3. sklearn: For computing cosine similarity.
4. Models: Pre-trained model all-MiniLM-L6-v2.

## Usage Instructions
1. Prepare the dataset (movies.csv) with columns: movieId, title, genres.
2. Generate embeddings for movie descriptions.
3. Input a natural language query to retrieve movie recommendations.
4. Customize the number of recommendations (default is top 5).

## Project Goal
1. The primary objective is to explore the power of semantic embeddings for creating an intuitive and user-friendly movie recommendation engine based on natural language inputs.
