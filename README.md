# Movie-Recommendor-System
Overview
      This project is a Content-Based Movie Recommendation System that suggests movies similar to those a user has previously shown interest in. By analyzing movie attributes like genres, keywords, cast, and crew, this system provides personalized recommendations that align with the user's tastes.
      
Installation
  1. Clone the repository: git clone https://github.com/ankitatiwari44/Movie-Recommendor-System
  2. Add Project directory: cd movie-recommendation
  3. Install required dependencies: pip install -r requirements.txt
     
 Data
  This project uses the IMDB dataset for training and testing. The dataset includes information such as movie titles, genres,   and user ratings.

Files:
tmdb_5000_movies: Contains movie IDs, budget, popularity, title, avg_votes, genres etc.
tmdb_5000_credits: Contains , movie_id, title, and crew.

Preprocessing
  The following preprocessing steps are applied:
    Extract and preprocess features such as genres, cast, director, and keywords.
    Combine these features into a single text field for each movie.
    Use text vectorization (TF-IDF or Count Vectorizer) to create a matrix of movie features.

Usage
  Run the Application:
    If using Streamlit: streamlit run app.py

Recommendation Approach
  This recommendation system uses a content-based filtering approach:
    #Feature Extraction: Extracts relevant movie information (e.g., genres, keywords, cast, and director) and combines them into a unified text representation.
    #Text Vectorization: Transforms the combined text data into vectors using TF-IDF (Term Frequency-Inverse Document Frequency) to give more weight to unique terms.
    #Similarity Calculation: Computes similarity between movies using cosine similarity, which measures the angle betwee two feature vectors
Results
  The system's recommendations are evaluated based on user satisfaction
  Relevance: Most recommended movies are in line with user preferences.
  Example Recommendations:
  If a user likes The Dark Knight, recommendations might include Batman Begins and V for Vendetta.
[app.pdf](https://github.com/user-attachments/files/17774197/app.pdf)


  
