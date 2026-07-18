# 🎬 Movie Recommender System

A Machine Learning-based web application that provides intelligent movie suggestions using content-based filtering. The application uses a trained recommendation model built in a Jupyter Notebook and provides an interactive dashboard using Streamlit.

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subodh-movie-recommender-system.streamlit.app)

## 📌 Project Overview
This project recommends similar movies based on user selection. It calculates the feature similarities (like genres, keywords, cast, and crew vectors) using text vectorization and cosine similarity. The repository contains the data analysis/modeling pipeline inside a Jupyter Notebook and exposes the user interface through a lightweight Streamlit app.

## 🚀 Features
- **Smart Recommendations:** Leverages machine learning cosine similarity matrix calculations to recommend the top most similar movies.
- **Interactive Web Interface:** A smooth dropdown experience built completely with Streamlit.
- **Data Exploration:** Includes an `.ipynb` notebook file capturing the full model training and evaluation process.

## 🛠️ Tech Stack
- **Python** (Core language)
- **Jupyter Notebook** (Model prototyping & data exploration)
- **Streamlit** (Web application framework)
- **Pandas & NumPy** (Data processing and cleaning)
- **Scikit-learn** (Feature extraction & similarity scoring)

## 📂 Project Structure
```text
movie-recommender-system/
│── app.py                   # Main Streamlit web application
│── movie_recommender.ipynb  # Jupyter Notebook with data analysis & ML modeling
│── requirements.txt         # Configuration file listing all dependencies
│── README.md                # Project documentation

---

## ⚙️ Installation

Clone the repository:

```bash
git clone [https://github.com/subodh138/movie-recommender-system.git](https://github.com/subodh138/movie-recommender-system.git)
```

Navigate to the project folder:

```bash
cd movie-recommender-system
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment.

**Windows**

```bash
venv\Scripts\activate
```

**Linux/macOS**

```bash
source venv/bin/activate
```

Install the required packages:

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Application

Start the Flask server:

```bash
streamlit run app.py
```

Open your browser and visit:

```text
http://localhost:8501
```

---

## 🧠 Recommendation Algorithm

This project uses **Content-Based Filtering**.

### Workflow

1. Load the movie dataset.
2. Extract movie genres.
3. Convert genres into TF-IDF vectors.
4. Compute cosine similarity between movies.
5. Recommend the top five most similar movies.

---

## 📊 Dataset

The system is trained using the **TMDB 5000 Movie Dataset**, analyzing complex metadata points including:

Dataset includes:

* Movie Titles & Plots
* Genres & Keywords
* Production Cast & Crew lists

---

## 🌐 Deployment

This application can be deployed on **Streamlit Community Cloud** using:

- **Deployment Platform:** Streamlit Share
- **Runtime Environment:** Python 3.12 (or 3.11 depending on your selection)
- **Main Entrypoint:** `app.py`

  
## 📈 Future Improvements

**Fetch Movie Posters:** Integrate the **TMDb API** to fetch and display official movie posters next to the recommendations.
**Search Autocomplete:** Add a smart search bar that suggests movie titles as the user types.
**Detailed Movie Info:** Add a feature to show the movie overview, release date, and user ratings when a recommended movie is clicked.
**Hybrid Recommendation:** Combine content-based filtering with collaborative filtering (user ratings) for more personalized suggestions.

---

## 📄 License

This project is developed for educational and portfolio building purposes.
