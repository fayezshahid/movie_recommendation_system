# Movie Recommendation System

A content-based movie recommendation system that analyzes movie attributes (genre, plot, cast, keywords) to provide personalized movie recommendations using advanced filtering algorithms.

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation
- **Scikit-learn** - Machine learning and text processing
- **Streamlit** - Web interface
- **CountVectorizer** - Text feature extraction
- **Cosine Similarity** - Similarity measurement

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/fayezshahid/movie_recommendation_system.git
   cd movie_recommendation_system
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Get similarity.pkl file**
   
   **Note:** `similarity.pkl` is not included in the git repo because of its size.
   
   **Option 1:** Train the model yourself
   ```bash
   # Run the Jupyter notebook to generate similarity.pkl
   jupyter notebook Main.ipynb
   ```
   
   **Option 2:** Download pre-trained model
   ```
   Download similarity.pkl from Google Drive:
   [https://drive.google.com/file/d/1r6UoLbzEo6jK4cYVyTucCZRSUUqZueNy/view]
   ```

## 💻 Usage

1. **Launch the web app**
   ```bash
   streamlit run app.py
   ```

2. **Use the interface**
   - Select a movie from the dropdown
   - Click "Show Recommend" to get 5 similar movies

## 🔧 How It Works

1. **Data Processing**: Combines movie overview and genre into 'tags'
2. **Vectorization**: Converts text to numerical vectors using CountVectorizer
3. **Similarity**: Calculates cosine similarity between all movies
4. **Recommendation**: Returns top 5 most similar movies


## 🎯 Features

- Content-based filtering algorithm
- Interactive web interface with Streamlit
- Processes 10,000+ text features
- Fast recommendations using pre-computed similarity matrix
