# 🎵 Mini Music Predictor

A simple machine learning project that predicts music genres based on user attributes using a decision tree classifier.

---

## 📌 Overview

This project demonstrates how to train and use a **Decision Tree** model to predict music genres based on a user's age and gender. It's a beginner-friendly ML project using Python, scikit-learn, and Jupyter Notebook.

---

## 📁 Repository Structure

-   `index.ipynb` – Jupyter Notebook with code for loading data, training the model, and making predictions.
-   `music.csv` – Dataset used to train the model.
-   `music-recommender.joblib` – Serialized model for making predictions.
-   `music-recommender.dot` – Graphviz file used to visualize the decision tree.

---

## 🚀 Getting Started

### ✅ Prerequisites

-   Python 3.x
-   Jupyter Notebook
-   Required Python packages:
    -   pandas
    -   scikit-learn
    -   joblib
    -   graphviz (for visualization)

### 💻 Installation

1.  **Clone the repository**

    ```bash
    git clone [https://github.com/snehauppula/Mini-musicPredictor.git](https://github.com/snehauppula/Mini-musicPredictor.git)
    cd Mini-musicPredictor
    ```

2.  **Install the packages**

    ```bash
    pip install pandas scikit-learn joblib graphviz
    ```

3.  **Launch Jupyter Notebook**

    ```bash
    jupyter notebook index.ipynb
    ```

---

## 🧠 How It Works

The dataset (`music.csv`) contains user information: **Age**, **Gender**, and their preferred **music genre**.

A **Decision Tree Classifier** is trained on this data.

The model is saved using `joblib` and can later be used for predictions.

The structure of the decision tree is exported to a `.dot` file for visualization.

---

## 🎯 Sample Prediction

Once the model is trained:

```python
model.predict([[21, 1]])  # Predicts music preference for a 21-year-old male (assuming 1 represents male)
