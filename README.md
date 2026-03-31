# Netflix Movie Recommendation System

## Project Overview  

This project is a content-based movie recommendation system built using the Netflix Movies & TV Shows dataset (~8,800 titles). The system recommends movies similar to a selected title by analyzing textual features such as plot descriptions and genre tags.

The goal of this project is to demonstrate how Natural Language Processing (NLP) techniques can be applied to build an intelligent recommendation engine and integrate it with an interactive user interface.

---

## Problem Statement  

With the rapid growth of streaming platforms, users often face difficulty in discovering relevant content. This project addresses the problem by building a recommendation system that suggests movies based on content similarity rather than user history.

---

## Dataset  

- Source: Kaggle Netflix Movies & TV Shows Dataset  
- Total Titles: 8,807  
- Features Used:
  - Title  
  - Description  
  - Genre (listed_in)  
  - Rating  
  - Release Year  

---

## Approach  

### 1. Data Preprocessing  
- Handled missing values  
- Removed duplicates  
- Standardized genre formats  
- Combined genres and descriptions into a single text feature ("soup")  

### 2. Feature Engineering  
- Tokenization and stopword removal  
- Removal of rare and overly frequent terms  
- Creation of a unified textual representation  

### 3. Vectorization (TF-IDF)  
- Converted text into numerical vectors using TF-IDF  
- Captured importance of words relative to the dataset  

### 4. Similarity Computation  
- Used cosine similarity to compute similarity between movies  
- Built a similarity matrix across all titles  

### 5. Recommendation System  
- Given a movie, returns Top-N most similar titles  
- Supports filtering by:
  - Genre  
  - Rating  
  - Release Year  

---

## Features  

- Content-based recommendation engine  
- Real-time movie recommendations  
- Interactive filtering options  
- Clean and responsive UI  
- Integrated EDA visualizations  

---

## Exploratory Data Analysis (EDA)  

Key insights derived from the dataset:

- International Movies and Dramas dominate the catalog  
- Rapid content growth observed between 2015–2018  
- Majority of content falls under TV-MA and TV-14 ratings  
- Minimal missing values in key features used for modeling  

---

## Tech Stack  

- **Frontend:** HTML, CSS, JavaScript  
- **Visualization:** Chart.js  
- **Backend Logic:** Python (Google Colab)  
- **Machine Learning / NLP:**  
  - TF-IDF Vectorization  
  - Cosine Similarity  

---

## How It Works  

1. User selects a movie  
2. System retrieves its TF-IDF vector  
3. Cosine similarity is computed against all other movies  
4. Top-N similar movies are ranked and displayed  
5. Filters refine the results based on user preference  

---

## Project Structure  
├── notebook.ipynb # Main ML model and preprocessing
├── index.html # Frontend UI
├── README.md # Project documentation


---

## Future Improvements  

- Hybrid recommendation system (content + collaborative filtering)  
- Integration with real-time APIs  
- Deployment using Flask or FastAPI  
- Personalized recommendations based on user history  

---

## Learning Outcomes  

- Built a recommendation system from scratch  
- Applied NLP techniques on real-world data  
- Understood TF-IDF and cosine similarity in depth  
- Gained experience in data preprocessing and feature engineering  
- Developed an end-to-end data science project with UI integration  

---

## Conclusion  

This project demonstrates how machine learning and NLP techniques can be used to build scalable recommendation systems. By combining data analysis, feature engineering, and interactive visualization, the system provides meaningful and efficient movie recommendations.
