# Movie-Recommendation-System

## Project Overview

This project develops a personalized Movie Recommendation System for the Streamora OTT platform. The system recommends movies based on previously watched movies by using movie titles, genres, and descriptions to understand content similarity.

The main objective is to provide more relevant movie recommendations and improve user engagement.

## Objective

* Recommend movies based on user viewing history.
* Understand semantic similarity between movies.
* Provide personalized movie suggestions.
* Compare different recommendation approaches.
* Build an interactive recommendation interface.

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Gensim
* Sentence Transformers
* Cosine Similarity
* Gradio
* Matplotlib
* Seaborn
* Google Colab

## Project Workflow

1. Load and preprocess the movie dataset.
2. Combine movie title, genres, and overview.
3. Generate movie embeddings using Sentence Transformer.
4. Calculate similarity using Cosine Similarity.
5. Use previously watched movies as user preferences.
6. Generate the top 10 movie recommendations.
7. Evaluate recommendation performance.
8. Create an interactive Gradio interface.

## Recommendation Approach

### Sentence Transformer

The project uses the pretrained `all-MiniLM-L6-v2` Sentence Transformer model.

The model converts movie information into numerical embeddings that capture the semantic meaning of the movie content.

Cosine Similarity is then used to compare movie embeddings and identify movies with similar content.

## Recommendation Logic

The `recommend_movies_sentf()` function takes the user's watched movie titles and:

* Finds the corresponding movies.
* Generates embeddings for the watched movies.
* Calculates similarity with other movies.
* Ranks movies based on similarity.
* Returns the top 10 recommendations.

## Interactive Interface

A Gradio interface is implemented to allow users to select movies and receive personalized recommendations.

The interface accepts movie selections and displays the recommended movie titles.

## Model Evaluation

The project evaluates recommendation performance using past movie-watching data.

Monthly and overall success percentages are calculated to measure recommendation performance. The project also compares Word2Vec and Sentence Transformer based recommendation approaches.

## Key Features

* Personalized movie recommendations
* Semantic similarity-based recommendations
* Sentence Transformer embeddings
* Cosine Similarity
* Top 10 movie recommendations
* Word2Vec comparison
* Interactive Gradio interface
* Recommendation performance evaluation

## Project Structure

```text
Movie-Recommendation-System/
│
├── Movie_Recommendation_system.ipynb
├── README.md
└── dataset/
    └── movie_dataset.csv
```

## Conclusion

This project demonstrates how NLP embeddings and semantic similarity can be used to develop a personalized movie recommendation system. Sentence Transformer helps understand movie content and generate relevant recommendations based on users' viewing history.


