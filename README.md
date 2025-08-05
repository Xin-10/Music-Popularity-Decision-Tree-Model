# Music-Popularity-Decision-Tree-Model

This project investigates whether the popularity of a song on Spotify can be predicted using audio and metadata features.  
Using a dataset of over 114,000 songs across 125 genres, tree-based machine learning models were applied to classify tracks as "popular" or "not popular" and to predict their actual popularity scores.

## Models Used

- **Decision Tree Classifier**  
  Classifies songs into "popular" or "not popular" categories.  
  Accuracy: 72.7%.  
  Top features: `popular_genre_1`, `acousticness`, `valence`, `duration_min`.

- **Random Forest Classifier**  
  Improves performance and stability.  
  Accuracy: 78.4%.  
  Top features: `valence`,  `acousticness`，`duration_min`，`tempo`.  
  Genre popularity contributed less due to averaging in ensemble learning.

- **Decision Tree Regressor**  
  Predicts actual popularity scores (0–100).  
  R² score ≈ 0.10 → limited predictive power.

## Installation & Execution

This project runs on **Python 3.12+** and requires several dependencies listed in `requirements.txt`.

### 1. Clone the repository
```bash
git clone https://github.com/Xin-10/Music-Popularity-Decision-Tree-Model.git
cd Music-Popularity-Decision-Tree-Model
```

## 2. Create a virtual environment (Recommended)
```bash
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate      # Windows
```

## 3. Install dependencies
```bash
pip install -r requirements.txt
```

## 4. Launch Notebook and Run
```bash
jupyter notebook
Then open and run A2_tree_music_popularity.ipynb
```
