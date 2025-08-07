# Movie-Recommender-System
A content-based movie recommendation system built using Python, Streamlit, and TMDb API. This project helps users discover movies similar to the ones they already like — by analyzing metadata like genres, cast, director, and plot tags.

## Features

- Search any movie and get 5 personalized recommendations
- Displays movie posters using TMDb API
- Fast and interactive UI using Streamlit
- Precomputed cosine similarity matrix for real-time response
- Styled dark theme interface with custom CSS
- Handles missing posters or API failures gracefully

## Dataset Used

Combined **Movies** and **Credits** datasets from Kaggle:
- Merged on `movie_id`
- Extracted: title, overview, genres, keywords, cast, crew
- Created a combined `tags` column for text-based similarity

## Tech Stack

- **Python**
- **pandas**, **scikit-learn**, **pickle**
- **Streamlit** for UI
- **TMDb API** for fetching posters
- **CountVectorizer** + **Cosine Similarity** for recommendations

## How It Works

1. User selects a movie title from the dropdown.
2. System retrieves its vector and computes cosine similarity with all other movies.
3. Top 5 similar movies are recommended.
4. Posters fetched using movie IDs via the TMDb API.

## Installation & Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/movie-recommender.git
   cd movie-recommender

## Live App:https://movie-recommender-system-iq2f.onrender.com/
