# 🎬 CineMatch - Movie Recommendation System

CineMatch is a full-featured, content-based movie recommendation web application powered by **FastAPI**, **Streamlit**, **Scikit-Learn**, and the **TMDB API**. It features a robust backend API serving recommendations using TF-IDF vectorization and cosine similarity, paired with an interactive, modern user interface.

---

## ✨ Features

- **Personalized Recommendations:** Get similar movie suggestions instantly based on content analysis (genres, overview, cast, crew).
- **FastAPI Backend:** High-performance asynchronous API handling movie search, metadata, and recommendation computation.
- **Streamlit Frontend:** Clean, responsive, multi-view UI supporting grid layouts, movie details pages, posters, cast information, and trailers.
- **TMDB Integration:** Fetches real-time movie posters, backdrops, ratings, runtime, and cast details using TMDb API.

---

## 🛠️ Tech Stack

- **Backend:** FastAPI, Uvicorn, Python, Pandas, NumPy, Scikit-Learn, Scipy
- **Frontend:** Streamlit, HTML/CSS
- **External API:** The Movie Database (TMDB) API

---

## 📂 Project Structure

```text
movies-recommendation-system/
│
├── app.py              # Streamlit frontend UI application
├── main.py             # FastAPI backend server
├── movies.ipynb        # Jupyter notebook for data preprocessing & EDA
├── movies_metadata.csv # Raw/Processed dataset source
├── requirements.txt    # Project dependencies
├── df.pkl              # Pickled dataframe of movie metadata
├── indices.pkl         # Pickled movie title-to-index mappings
├── tfidf.pkl           # Pickled TF-IDF vectorizer model
├── tfidf_matrix.pkl    # Pickled TF-IDF feature matrix
└── runtime.txt         # Python version configuration
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10 or higher
- A TMDb API Key ([Get one here](https://www.themoviedb.org/settings/api))

### 1. Clone the Repository
```bash
git clone https://github.com/GaganYadav20/movies-recommendation-system.git
cd movies-recommendation-system
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Environment Configuration
Create a `.env` file in the root directory and add your TMDb API Key:
```env
TMDB_API_KEY=your_tmdb_api_key_here
```

### 4. Run the Application

**Run the FastAPI Backend:**
```bash
uvicorn main:app --reload --port 8000
```

**Run the Streamlit Frontend (in a separate terminal):**
```bash
streamlit run app.py
```

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

