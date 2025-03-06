# Movie Recommendation System

## 📌 Overview
This project is a **Movie Recommendation System** that suggests similar movies based on a given movie title. It uses **Natural Language Processing (NLP)** techniques and **cosine similarity** to measure the closeness of movie descriptions, genres, keywords, cast, and crew.

## 📊 Dataset
- **TMDB 5000 Movies Dataset**
- Contains movie metadata including **title, overview, genres, cast, crew, and keywords**.
- Data cleaned and processed before applying vectorization.

## ⚙️ Features
- **Content-Based Filtering**: Recommends movies based on similarity in descriptions, genres, and keywords.
- **Cosine Similarity**: Measures the similarity between movies using **TF-IDF vectorization**.
- **Accuracy Evaluation**: Computes the accuracy of recommendations using similarity scores.

## 🚀 Technologies Used
- **Python**
- **Pandas, NumPy** (Data Processing)
- **Scikit-Learn** (Vectorization & Similarity Calculation)
- **Pickle** (Model & Data Serialization)

## 🔧 How It Works
1. **Data Preprocessing**:
   - Extracts **genres, keywords, cast, and crew**.
   - Cleans text data for better vectorization.
2. **Feature Extraction**:
   - Uses **CountVectorizer** to convert text into numerical vectors.
   - Computes **cosine similarity** between movies.
3. **Recommendation System**:
   - Given a movie title, it finds the **top 5 most similar movies**.
4. **Evaluation**:
   - Measures accuracy using a **threshold-based similarity scoring**.

## 📂 Files & Directories
```
│── movie_recommendation_cosine_similarities.ipynb  # Jupyter Notebook with code
│── tmdb_5000_movies.csv                            # Movie metadata
│── tmdb_5000_credits.csv                           # Cast & Crew data
│── movie_list.pkl                                  # Serialized movie data
│── similarity.pkl                                  # Cosine similarity matrix (not included due to size)
```

## 🛠 How to Run
```bash
# Clone the repository
git clone https://github.com/Salomiairy11/Recommend-Movie-System.git
cd Recommend-Movie-System

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter Notebook
jupyter notebook
```

## 🎯 Example Usage
```python
recommend('Inception')
# Output:
# 1. The Prestige
# 2. Interstellar
# 3. The Dark Knight Rises
# 4. Memento
# 5. Shutter Island
```

## 📝 Notes
- **`similarity.pkl`** is excluded due to GitHub’s 100MB limit. You need to regenerate it by running the notebook.
- Ensure all dependencies are installed before running the script.

## 📌 Future Improvements
- Improve accuracy with **TF-IDF** instead of CountVectorizer.
- Include user-based collaborative filtering.
- Deploy as a **Flask Web App**.

## 💡 Credits
- Dataset: **The Movie Database (TMDB)**.
- Developed by **@Salomiairy11**.

---
🎬 *Find your next favorite movie!* 🍿





