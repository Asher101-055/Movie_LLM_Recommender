movie recommender System

This project is a hybrid movie recommender system using both content-based filtering (with TF-IDF and cosine similarity) and collaborative filtering (using SVD from the Surprise library). It includes data exploration, model training, and deployment-ready model saving.

## Features

- **Content-based filtering:** Recommends movies based on genre similarity.
- **Collaborative filtering:** Predicts user ratings using SVD.
- **Hybrid recommendations:** Combines both approaches for better results.
- **Data visualization:** Explore rating distributions and top movies.
- **Model export:** Saves trained models for deployment.
- **Gradio/Streamlit ready:** Can be integrated with web UIs for interactive recommendations.

## Project Structure

```
movie_recommender/
│
├── data/                # Processed data files (e.g., movies.csv)
├── models/              # Saved model files (e.g., svd.pkl, cosine_sim.pkl)
├── notebook/
│   └── code.ipynb       # Main Jupyter notebook for exploration and training
├── app/                 # (Optional) Web app code (Gradio/Streamlit)
└── README.md            # Project documentation
```

## How to Run

1. **Install dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

2. **Prepare data:**
    - Place the MovieLens 1M dataset in `data/movielens_1m/` or update paths in the notebook.

3. **Run the notebook:**
    - Open `notebook/code.ipynb` in Jupyter or VS Code and run all cells.

4. **Train and save models:**
    - The notebook will save models to the `models/` directory.

5. **(Optional) Run the web app:**
    - For Gradio:  
      ```sh
      python app/gradio_app.py
      ```
    - For Streamlit:  
      ```sh
      streamlit run app/recommender_app.py
      ```

## Notes

- Large files (datasets, `.pkl` models) should be excluded from GitHub using `.gitignore`.
- Update paths as needed for your environment.
- For questions or improvements, open an issue or pull request.
