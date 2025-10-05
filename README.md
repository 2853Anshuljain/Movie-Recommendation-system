Movie Recommendation System
This project is a content-based movie recommendation system that suggests movies to users based on their similarity. The recommendation engine is built using Python, and the user interface is created with Streamlit.

Features
Content-Based Filtering: Recommends movies based on plot summaries, genres, keywords, cast, and crew.

Interactive UI: A user-friendly web interface built with Streamlit that allows users to select a movie and get recommendations.

Dynamic Poster Fetching: Fetches and displays movie posters from The Movie Database (TMDb) API to provide a richer user experience.

How It Works
The recommendation system works by creating a "tag" for each movie that combines its overview, genres, keywords, top 3 cast members, and director. These tags are then vectorized using the CountVectorizer to create a numerical representation of each movie. The cosine similarity between these vectors is then calculated to determine how similar the movies are to each other.

When a user selects a movie, the system finds the most similar movies and displays them as recommendations.

Files in This Project
movie-recommender system.ipynb: The Jupyter notebook containing all the data cleaning, preprocessing, and model building steps.

app.py: The Streamlit application that provides the user interface for the recommendation system.

movie_dict.pkl: A serialized dictionary containing the movie data.

similarity.pkl: A serialized file containing the cosine similarity matrix.

How to Run
Clone the repository:

git clone (https://github.com/2853Anshuljain/movie-recommendation-system.git)

Install the required libraries:

pip install -r requirements.txt

Run the Streamlit app:

streamlit run app.py

Open your web browser and go to the local URL provided by Streamlit to start using the recommendation system.

Libraries Used
Pandas: For data manipulation and analysis.

NumPy: For numerical operations.

Scikit-learn: For vectorizing text data and calculating cosine similarity.

NLTK: For natural language processing tasks like stemming.

Streamlit: For creating the interactive web application.

Requests: For making API calls to fetch movie posters.
