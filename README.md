# 🎬 Movie Recommender System

This is a **content-based movie recommender system** built using **Streamlit**, **Pandas**, and **The Movie Database (TMDb) API**. You can select a movie, and it will recommend five similar movies along with their posters.

---

## 📦 Features

- Select a movie from the dropdown list
- Get 5 similar movie recommendations
- Displays movie posters using TMDb API

---

## 🛠️ Tech Stack

- Python 🐍
- Streamlit 🎈
- Pandas 📊
- Pickle 🧪
- Requests 🌐
- TMDb API 🎞️

---

## 📁 Project Structure

```bash
.
├── app.py                 # Main Streamlit app
├── movie_dict.pkl         # Movie metadata dictionary
├── similarity.pkl         # Precomputed similarity matrix
├── README.md              # Project documentation
├── dataset                # Folder containing the dataset files
├── Procfile               # Movie metadata dictionary
├── MovieRecommender       # Jupyter Notebook 
├── requirements           # Dependency libraries


---

## 🧠 How It Works 

- Loads **movie metadata** and **similarity scores** from pickle files  
- Uses a **content-based filtering** approach (e.g., cosine similarity)  
- Calls **TMDb API** to fetch movie posters  
- Displays the results using **Streamlit**

---

## 🔧 Setup Instructions

1. **Clone the repo**

   ```bash
   git clone https://github.com/yourusername/movie-recommender.git
   cd movie-recommender

2. Install dependencies

3. Add your TMDb API key

Replace the value of api_key in app.py with your TMDb API key

api_key = "YOUR_API_KEY_HERE"
You can get one from The Movie Database.

4. Run the app

streamlit run app.py

📸 Example

Once you select a movie and hit Recommend, you’ll see five movie suggestions with their posters displayed side-by-side.

## 📌 Notes

Make sure the files movie_dict.pkl and similarity.pkl are in the same directory.

This model is based on content similarity, not user behavior.

## 💡 Future Improvements

Add user-based collaborative filtering

Include ratings and genres in the recommendation logic

Enhance UI/UX with more filters (year, genre, etc.)

Deploy on Streamlit Cloud or Render
