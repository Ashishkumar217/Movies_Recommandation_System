# 🎬 Movie Recommendation System

A **Content-Based Movie Recommendation System** built using **Machine Learning**, **Natural Language Processing (NLP)**, and **Streamlit**. The application recommends movies similar to a user's selected movie by analyzing movie metadata and calculating cosine similarity between feature vectors. The project uses the **TMDB 5000 Movies Dataset** and provides an interactive web interface for exploring recommendations.

---

## 📌 Features

* 🎥 Content-based movie recommendation
* 🔍 Search and select movies from an interactive dropdown
* 🤖 Cosine Similarity-based recommendation engine
* ⚡ Fast recommendation generation using a precomputed similarity matrix
* 🌐 Interactive web application built with Streamlit
* 🧠 NLP-based feature engineering using movie metadata
* 🖼️ Support for movie posters using the TMDB API (optional)

---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Machine Learning:** Scikit-learn
* **Data Manipulation:** Pandas, NumPy
* **Web Framework:** Streamlit
* **API:** TMDB API (Optional for Posters)
* **Serialization:** Pickle

---

## 📂 Project Structure

```text
Movies_Recommandation_System/
│
├── app.py                     # Streamlit application
├── Movie_Recommendation_System.ipynb
├── movie_data.pkl             # Processed movie data & similarity matrix
├── tmdb_5000_movies.csv       # Movie dataset
├── tmdb_5000_credits.csv      # Credits dataset
├── requirements.txt
└── README.md
```

---

## 📊 Dataset

This project uses the **TMDB 5000 Movies Dataset**, which contains movie metadata such as:

* Movie Title
* Genres
* Overview
* Cast
* Crew
* Keywords
* Production Companies

The recommendation engine combines these features into a single text representation ("tags") and computes similarity scores using **CountVectorizer** and **Cosine Similarity**.

---

## ⚙️ How It Works

1. Load the TMDB Movies and Credits datasets.
2. Merge both datasets.
3. Perform data cleaning and preprocessing.
4. Extract important features:

   * Genres
   * Keywords
   * Cast
   * Director
   * Overview
5. Create a combined **tags** column.
6. Convert text into vectors using **CountVectorizer**.
7. Compute **Cosine Similarity** between all movies.
8. Recommend the Top 10 most similar movies.

---

## 🚀 Installation

### Clone the repository

```bash
git clone https://github.com/Ashishkumar217/Movies_Recommandation_System.git
cd Movies_Recommandation_System
```

### Create a virtual environment (Optional)

**Windows**

```bash
python -m venv .venv
.venv\Scripts\activate
```

**Linux / macOS**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

Open your browser and visit:

```
http://localhost:8501
```

---

## 📸 Application Preview

Add screenshots of your application here.

Example:

```
assets/
├── home.png
├── recommendations.png
```

Then embed them:

```markdown
![Home Screen](assets/home.png)

![Recommendations](assets/recommendations.png)
```

---

## 📈 Machine Learning Pipeline

```
TMDB Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Feature Engineering
      │
      ▼
Tags Creation
      │
      ▼
CountVectorizer
      │
      ▼
Cosine Similarity Matrix
      │
      ▼
Top 10 Movie Recommendations
```

---

## 📚 Libraries Used

* Streamlit
* Pandas
* NumPy
* Scikit-learn
* Requests
* Pickle

---

## 🔮 Future Improvements

* User authentication
* Genre-based filtering
* Hybrid recommendation system
* Collaborative filtering
* Deep learning-based recommendations
* Movie trailer integration
* IMDb ratings and reviews
* Deploy on Streamlit Community Cloud

---

## 🤝 Contributing

Contributions are welcome!

If you have ideas to improve this project:

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Open a Pull Request.

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Ashish Saini**

* GitHub: https://github.com/Ashishkumar217
* LinkedIn: *(Add your LinkedIn profile here if you'd like.)*

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub. It helps others discover the project and motivates further development.
