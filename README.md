#  Movie Recommender App

A web-based Movie Recommender System built with **Streamlit**, trained using collaborative filtering, and hosted using **Streamlit Cloud**. Large assets like similarity matrices are loaded from [Hugging Face Hub](https://huggingface.co/).

![App Screenshot](https://github.com/varunsathaye/movie-recommender/blob/main/ss.png)

---

## 🔗 Live Demo

👉 [Click here to try the app](https://igivemovies.streamlit.app)

---

##  Features

-  **Search** for a movie by title
-  **Top 5 Recommendations** using vector similarity
-  Trained on movie data with collaborative filtering
-   Fast loading using Hugging Face-hosted assets

---

##  Tech Stack

- **Frontend & App:** [Streamlit](https://streamlit.io/)
- **Backend:** Python, Pandas, Pickle, SciKitLearn
- **Model Assets Hosting:** [Hugging Face Hub](https://huggingface.co/)
- **Deployment:** [Streamlit Cloud](https://streamlit.io/cloud)

---

##  Challenges Faced

-The data I received from the dataset was quite messy. I had to clean it up using various pre processing steps. Some irrelevant features were dropped.
- GitHub has a 100 MB file limit, which made it impossible to store large `.pkl` files in the repo. I solved this by hosting the files on [Hugging Face Hub](https://huggingface.co/), which also made them easier to download in the Streamlit app.
- Streamlit Cloud doesn't allow direct access to local storage like Google Drive, so I had to find a way to make model files available via HTTP.
- Initially ran into errors trying to `pickle.load()` files from URLs — solved it using `io.BytesIO` for byte stream handling.

> Each roadblock helped me better understand how to combine web app development with scalable data storage.

---
