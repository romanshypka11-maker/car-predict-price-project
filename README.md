# 🚗 Car Price AI Assistant
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange)
![ML](https://img.shields.io/badge/Machine%20Learning-XGBoost-green)
![NLP](https://img.shields.io/badge/NLP-SentenceTransformers-yellow)
## Car Price AL Assistant is a system for searching for cars by price. Created for different groups of people who want to buy a car using natural language.
This project is a comprehensive study of the used car market. The main goal is to build tools for automatic vehicle valuation and "smart" semantic search based on natural language descriptions.

This notebook (`.ipynb`) demonstrates an end-to-end Data Science workflow: from data cleaning and feature engineering to building Machine Learning models and a Vector Database.

## 🛠️ Tech Stack
* **Python 3.10**
* **Pandas & NumPy** — Data manipulation and analysis.
* **Matplotlib & Seaborn** — Data visualization (EDA).
* **Scikit-Learn / XGBoost** — Regression models for price prediction.
* **ChromaDB** — Vector database for semantic search.
* **SentenceTransformers** — NLP model (`all-MiniLM-L6-v2`) for generating text embeddings.

## 📊 Key Workflow Stages

### 1. Data Wrangling & Preprocessing
* Cleaned the dataset by removing duplicates and handling missing values.
* Managed outliers in `Price` and `Mileage` columns.
* Performed Feature Engineering (creating new features, categorical encoding).

### 2. Exploratory Data Analysis (EDA)
* Visualized price distributions.
* Analyzed correlations between mileage, car age, engine size, and price.

### 3. Machine Learning (Price Prediction)
* Trained an **XGBoost Regressor** to predict car prices.
* **Model Performance:**
    * MAE (Mean Absolute Error): `~$ [Insert Your MAE]`
    * R² Score: `0.XX` (Insert your accuracy score)

### 4. Semantic Search (NLP + ChromaDB)
* Implemented a vector search engine using **ChromaDB**.
* Converted car descriptions into vector embeddings using **SBERT**.
* The system understands context-based queries (e.g., *"Cheap family car"*) and retrieves relevant results (Minivans, Station Wagons) even if exact keywords are missing.

## 🚀 How to Run
You can view the notebook directly on GitHub or run it locally.

1.  Clone the repository:
    ```bash
    git clone [https://github.com/YOUR_USERNAME/REPO_NAME.git](https://github.com/YOUR_USERNAME/REPO_NAME.git)
    ```
2.  Install dependencies:
    ```bash
    pip install pandas numpy scikit-learn xgboost chromadb sentence-transformers seaborn matplotlib
    ```
3.  Launch Jupyter Lab/Notebook:
    ```bash
    jupyter lab
    ```

