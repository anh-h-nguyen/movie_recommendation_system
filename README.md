# 🎬 Movie Recommendation System  

## Technologies Used  
- Programming Language: Python  
- Libraries: Pandas, NumPy, Scikit-Learn, TfidfVectorizer  
- Algorithms: TF-IDF + Cosine Similarity  
- Dataset: MovieLens (movies, ratings, and tags)  

## Project Overview  
This Movie Recommendation System suggests personalized movie recommendations based on user input. By analyzing genres, ratings, and user-generated tags, it computes content-based similarity scores using TF-IDF vectorization and cosine similarity.  

Users can input a movie they love, and the system will suggest 10 similar movies based on content similarity and ratings data.  

## Purpose  
The system aims to:  
- Provide intelligent movie recommendations based on content and user-generated data.  
- Use text-based similarity (genres & tags) to find related films.  
- Incorporate rating data for more refined suggestions.  
- Allow interactive movie searching within a simple command-line interface.  

## How It Works  
1. Data Preprocessing  
   - Extracts TF-IDF features for movie genres.  
   - Aggregates user tags into a single descriptive string for each movie.  
   - Computes cosine similarity to find movies with overlapping content.  
   - Integrates average ratings to refine recommendations.  

2. User Interaction  
   - Users enter a movie title they enjoy.  
   - The system searches for matching movies.  
   - Using cosine similarity, it ranks the top 10 movies with similar characteristics.  
   - Users can input another movie or exit.  

## Design Approach  
- Text Cleaning: Standardized movie titles for matching consistency.  
- Balanced Similarity Calculation: Averaging genre-based and tag-based similarities.  
- Interactive CLI Experience: Users receive clear prompts & readable recommendations.  

## Ethical Considerations  
This recommendation system does not rely on user preferences beyond input titles. Instead, it suggests movies based on genre, tags, and ratings.  
Potential biases include:  
- Limited dataset scope (MovieLens may not reflect niche or indie films).  
- Tags availability (Some movies may lack user-generated tags, affecting accuracy).  
- Generalized similarity rather than personal preferences like favorite actors or directors.  

## Future Improvements  
- Enhance personal recommendations by incorporating collaborative filtering.  
- Integrate trending movies to mix popularity rankings with similarity scores.  
- Develop a web-based version for easy accessibility and visualization.  
- Refine tag processing by using NLP techniques like word embeddings.  
