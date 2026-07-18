# 🎬 Movie Recommendation System

An end-to-end content-based Movie Recommendation System built using Natural Language Processing (NLP), TF-IDF Vectorization, Cosine Similarity, FastAPI, Streamlit, and the TMDB API.

The system recommends movies based on the similarity of their content, including genres, keywords, cast, crew, overview, and other movie-related information.

---

## 🚀 Project Overview

Finding a good movie to watch can be difficult because of the huge number of available movies.

This project solves that problem by building a personalized movie recommendation system that recommends movies similar to a selected movie.

The project combines:

- Natural Language Processing (NLP)
- Text preprocessing
- TF-IDF Vectorization
- Cosine Similarity
- Content-based filtering
- FastAPI backend
- Streamlit frontend
- TMDB API integration

The system takes a movie title as input and returns similar movie recommendations along with movie details and posters.

---

## 🎯 Problem Statement

Users often spend a significant amount of time searching for movies they may enjoy.

Traditional movie search systems may only search by title. This project provides a content-based recommendation system that recommends movies based on the similarity between movie features.

For example:

> If a user selects `Inception`, the system can recommend movies with similar genres, keywords, storyline, cast, and other content features.

---

## ✨ Key Features

- 🎬 Movie search using TMDB API
- 🔍 Search for movies by title
- 🧠 Content-based movie recommendations
- 📝 NLP-based text preprocessing
- 📊 TF-IDF text vectorization
- 📐 Cosine similarity-based recommendation engine
- 🎞️ Movie posters and details using TMDB API
- 🎭 Genre-based recommendations
- ⚡ FastAPI REST API backend
- 🌐 Streamlit interactive web interface
- 🔄 Real-time movie search and recommendations
- 📦 Pre-trained recommendation resources stored using Pickle

---

## 🏗️ Project Architecture

```text
                    ┌──────────────────────┐
                    │       User           │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │   Streamlit UI       │
                    │    (Frontend)         │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │    FastAPI Backend   │
                    │      REST API        │
                    └──────────┬───────────┘
                               │
              ┌────────────────┴────────────────┐
              │                                 │
              ▼                                 ▼
   ┌──────────────────────┐          ┌──────────────────────┐
   │ Local ML Model       │          │     TMDB API         │
   │                      │          │                      │
   │ TF-IDF Vectorizer    │          │ Movie Search         │
   │ TF-IDF Matrix        │          │ Movie Details        │
   │ Cosine Similarity    │          │ Posters              │
   │                      │          │ Genres               │
   └──────────────────────┘          └──────────────────────┘
