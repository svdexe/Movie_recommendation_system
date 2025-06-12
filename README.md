# 🎬 Movie Recommendation System

<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white" alt="Scikit-learn"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="Pandas"/>
</div>

<br>

<div align="center">
  <img src="https://github.com/svdexe/Movie_recommendation_system/blob/main/website_output.png" alt="Movie Recommendation Interface" width="700"/>
  <p><em>Clean and intuitive movie selection interface showing Jurassic World recommendations</em></p>
</div>

<br>

## ✨ Features

🎯 **Smart Recommendations** · Get 5 personalized movie suggestions based on content similarity  
🖼️ **Movie Posters** · Visual display of recommended movies with poster images from TMDB API  
🎨 **Interactive UI** · Clean and intuitive Streamlit web interface  
📊 **ML-Powered** · Uses cosine similarity and TF-IDF vectorization for accurate recommendations  
🔍 **Content-Based Filtering** · Analyzes movie genres, keywords, cast, crew, and plot overview

## 🛠️ Tech Stack

**Python** · Core programming language  
**Streamlit** · Web application framework  
**Pandas** · Data manipulation and analysis  
**Scikit-learn** · Machine learning algorithms  
**NLTK** · Natural language processing  
**TMDB API** · Movie posters and metadata  
**Pickle** · Model serialization  

## 🚀 Quick Start

**Prerequisites**
```
Python 3.7+ · pip package manager
```

**Installation**
```bash
# Clone the repository
git clone https://github.com/yourusername/movie-recommendation-system.git
cd movie-recommendation-system

# Install dependencies
pip install streamlit pandas scikit-learn nltk requests pickle-mixin

# Download required data
python -c "import nltk; nltk.download('punkt')"

# Run the application
streamlit run app.py
```

Open your browser and navigate to `http://localhost:8501`

## 📁 Project Structure

```
movie-recommendation-system/
│
├── app.py                 # Main Streamlit application
├── movies_dict.pkl        # Preprocessed movie data
├── similarity.pkl         # Cosine similarity matrix
├── requirements.txt       # Python dependencies
├── README.md             # Project documentation
└── data/
    ├── tmdb_5000_movies.csv
    └── tmdb_5000_credits.csv
```

## 🔧 How It Works

**Data Preprocessing** · Merges movie and credits datasets · Extracts relevant features: genres, keywords, cast, crew, overview · Applies text preprocessing and stemming

**Feature Engineering** · Combines all text features into a single 'tags' column · Uses TF-IDF vectorization with 5000 max features · Removes English stop words

**Similarity Calculation** · Computes cosine similarity between all movies · Creates a similarity matrix for fast lookups

**Recommendation Generation** · Finds the selected movie's index · Retrieves top 5 most similar movies · Fetches movie posters from TMDB API

## 🎯 Algorithm Details

The recommendation system uses **Content-Based Filtering**

**Vectorization** · TF-IDF (Term Frequency-Inverse Document Frequency)  
**Similarity Metric** · Cosine Similarity  
**Features Used** · Movie overview, genres, keywords, cast, crew  
**Text Processing** · Porter Stemming, stop word removal  

## 📊 Dataset

**Source** · TMDB 5000 Movie Dataset  
**Movies** · 4,800+ movies  
**Features** · 20+ attributes per movie  
**Time Period** · Various years of cinema  

## 🔮 Future Enhancements

- [ ] **Hybrid Filtering** · Combine content-based with collaborative filtering
- [ ] **User Profiles** · Personalized recommendations based on viewing history
- [ ] **Advanced NLP** · Use word embeddings (Word2Vec, BERT) for better text understanding
- [ ] **Real-time Data** · Integration with live movie databases
- [ ] **Rating System** · Allow users to rate recommendations
- [ ] **Genre Filtering** · Filter recommendations by preferred genres
- [ ] **Mobile App** · React Native or Flutter mobile application

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

**CampusX** · for the comprehensive [original tutorial](https://www.youtube.com/watch?v=1YoD0fg3_EM&t=5947s) that served as the foundation for this project  
**TMDB** · for providing the movie database API  
**Kaggle** · for the movie dataset  
**Streamlit** · community for the amazing framework
 

## 📬 Contact

**Your Name** · shivamdali@gmail.com

Project Link: [https://github.com/yourusername/movie-recommendation-system](https://github.com/yourusername/movie-recommendation-system)

---

<div align="center">
  <p>⭐ Star this repo if you found it helpful!</p>
  <p>Made with ❤️ and lots of ☕</p>
</div>
