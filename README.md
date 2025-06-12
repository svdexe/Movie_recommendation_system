# 🎬 Movie Recommendation System

## 🖼️ Website Screenshot

<div align="center">
  <img src="https://github.com/svdexe/Movie_recommendation_system/blob/main/website_output.png" alt="Movie Recommendation Interface" width="800"/>
  <p><i>Clean and intuitive movie selection interface showing Jurassic World recommendations</i></p>
</div>


## ✨ Features

- 🎯 **Smart Recommendations**: Get 5 personalized movie suggestions based on content similarity
- 🖼️ **Movie Posters**: Visual display of recommended movies with poster images from TMDB API
- 🎨 **Interactive UI**: Clean and intuitive Streamlit web interface
- 📊 **ML-Powered**: Uses cosine similarity and TF-IDF vectorization for accurate recommendations
- 🔍 **Content-Based Filtering**: Analyzes movie genres, keywords, cast, crew, and plot overview

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **Python** | Core programming language |
| **Streamlit** | Web application framework |
| **Pandas** | Data manipulation and analysis |
| **Scikit-learn** | Machine learning algorithms |
| **NLTK** | Natural language processing |
| **TMDB API** | Movie posters and metadata |
| **Pickle** | Model serialization |

## 🚀 Quick Start

### Prerequisites
```bash
Python 3.7+
pip package manager
```

### Installation
1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/movie-recommendation-system.git
   cd movie-recommendation-system
   ```

2. **Install dependencies**
   ```bash
   pip install streamlit pandas scikit-learn nltk requests pickle-mixin
   ```

3. **Download required data**
   ```bash
   # Download NLTK data
   python -c "import nltk; nltk.download('punkt')"
   ```

4. **Run the application**
   ```bash
   streamlit run app.py
   ```

5. **Open your browser**
   Navigate to `http://localhost:8501`

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

### 1. **Data Preprocessing**
- Merges movie and credits datasets
- Extracts relevant features: genres, keywords, cast, crew, overview
- Applies text preprocessing and stemming

### 2. **Feature Engineering**
- Combines all text features into a single 'tags' column
- Uses TF-IDF vectorization with 5000 max features
- Removes English stop words

### 3. **Similarity Calculation**
- Computes cosine similarity between all movies
- Creates a similarity matrix for fast lookups

### 4. **Recommendation Generation**
- Finds the selected movie's index
- Retrieves top 5 most similar movies
- Fetches movie posters from TMDB API

## 🎯 Algorithm Details

The recommendation system uses **Content-Based Filtering**:

- **Vectorization**: TF-IDF (Term Frequency-Inverse Document Frequency)
- **Similarity Metric**: Cosine Similarity
- **Features Used**: Movie overview, genres, keywords, cast, crew
- **Text Processing**: Porter Stemming, stop word removal

## 📊 Dataset

- **Source**: TMDB 5000 Movie Dataset
- **Movies**: 4,800+ movies
- **Features**: 20+ attributes per movie
- **Time Period**: Various years of cinema


## 🔮 Future Enhancements

- [ ] **Hybrid Filtering**: Combine content-based with collaborative filtering
- [ ] **User Profiles**: Personalized recommendations based on viewing history
- [ ] **Advanced NLP**: Use word embeddings (Word2Vec, BERT) for better text understanding
- [ ] **Real-time Data**: Integration with live movie databases
- [ ] **Rating System**: Allow users to rate recommendations
- [ ] **Genre Filtering**: Filter recommendations by preferred genres
- [ ] **Mobile App**: React Native or Flutter mobile application


## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

🙏 Acknowledgments

TMDB for providing the movie database API
Kaggle for the movie dataset
Streamlit community for the amazing framework
Scikit-learn for machine learning tools
CampusX for the original tutorial that inspired this project 

## 📬 Contact

**Your Name** - shivamdali@gmail.com

Project Link: [https://github.com/yourusername/movie-recommendation-system](https://github.com/yourusername/movie-recommendation-system)

---

<div align="center">
  <p>⭐ Star this repo if you found it helpful!</p>
  <p>Made with ❤️ and lots of ☕</p>
</div>
