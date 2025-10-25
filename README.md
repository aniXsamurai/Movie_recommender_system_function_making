# 🎬 Movie Recommender System (Content-Based)

A **Content-Based Movie Recommendation System** built using Python and TMDB datasets, developed as part of the **Advanced Data Science** subject.  
The model recommends movies similar to a selected title by analyzing movie metadata such as **genres, keywords, cast, crew,** and **overview**.

---

## 📘 Project Overview

This project demonstrates the use of **Natural Language Processing (NLP)** and **machine learning techniques** for building a personalized recommendation engine.  
It uses **CountVectorizer** to represent movie content numerically and **Cosine Similarity** to measure similarity between movies.

---

## 🧠 Key Features

- Cleaned and merged **TMDB movie and credits datasets**
- Extracted and processed text-based metadata: genres, keywords, cast, crew
- Created combined "tags" representing each movie
- Vectorized using **CountVectorizer**
- Computed **Cosine Similarity** for similarity scoring
- Built a recommendation function to suggest top 5 similar movies

---

## 🗂️ Dataset

Source: [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

**Files used:**
- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

These datasets include information such as movie title, genres, keywords, overview, cast, and crew.

---

## ⚙️ Technologies Used

| Category | Libraries / Tools |
|-----------|-------------------|
| Programming | Python 3 |
| Data Handling | pandas, numpy |
| Text Processing | ast, sklearn (CountVectorizer) |
| Similarity Computation | sklearn (cosine_similarity) |
| Visualization | matplotlib, seaborn, wordcloud |
| Optional Deployment | Streamlit |

---

## 📊 Data Visualization

A few visual insights generated during data exploration:
- **Top Genres** — Count of movies per genre  
- **Top Actors and Directors** — Frequency of appearance  
- **Word Cloud** — Common words from movie overviews  
- **Similarity Heatmap** — Cosine similarity visualization for selected movies  

---

## 🧩 Model Workflow

```mermaid
flowchart TD
A[Load TMDB datasets] --> B[Data Cleaning & Preprocessing]
B --> C[Feature Extraction: genres, keywords, cast, crew]
C --> D[Create Combined 'Tags']
D --> E[Vectorization using CountVectorizer]
E --> F[Compute Cosine Similarity]
F --> G[Recommend Top 5 Similar Movies]
