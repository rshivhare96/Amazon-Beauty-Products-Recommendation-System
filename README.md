# 💄 Amazon Beauty Products Recommendation System

This project builds a **model-based collaborative filtering recommendation system** using user ratings for Amazon beauty products. The aim is to recommend relevant beauty items by uncovering hidden user preferences through **matrix factorization** techniques.

---

## 📂 Data

The dataset used for this project:

- `ratings_Beauty.csv`

### Key Features:

- **User ID** – Unique identifier for each user  
- **Product ID** – Unique identifier for each product  
- **Rating** – User-provided rating (1–5 scale)  
- **Timestamp** – Time of the rating event (optional for this project)

---

## 🔍 Workflow

The project follows a structured approach:

- **Data Preprocessing**:
  - Handling missing values
  - Filtering sparse users/items
  - Creating a **user-item utility matrix**

- **Dimensionality Reduction**:
  - Applying **Truncated Singular Value Decomposition (SVD)** to capture latent user-item interactions

- **Correlation Computation**:
  - Generating a **correlation matrix** to identify similar products

- **Recommendation Logic**:
  - For a given product, find highly correlated products
  - Filter out items already rated by the user

---

## 🎯 Key Outcomes

- Built a **personalized product recommender** based on user similarity in product ratings  
- Demonstrated effectiveness of **SVD** in capturing user preferences in sparse rating matrices  
- Showcased how product similarity can drive relevant recommendations  

---

## 📁 Notebook & Outputs

- `Amazon - Ratings (Beauty Products).ipynb`: Full pipeline from data loading to recommendation generation

Outputs include:

- Correlation heatmaps  
- List of top-N recommended products per user  
- Matrix visuals for utility and reduced dimensions  

---

## 🛠️ Libraries Used

- **Data Handling**: `pandas`, `numpy`  
- **Modeling**: `scikit-learn` (TruncatedSVD)  
- **Visualization**: `matplotlib`, `seaborn`  

---

## ✅ How to Use

1. Clone this repository  
2. Place `ratings_Beauty.csv` in the working directory  
3. Open and run `Amazon - Ratings (Beauty Products).ipynb`  
4. Modify the target product/user ID to generate customized recommendations  

---

## 🚀 Future Enhancements

- Incorporate **product metadata** (e.g., brand, category) for hybrid recommendations  
- Introduce **implicit feedback** like clicks or views  
- Deploy as a REST API or integrate into a user-facing dashboard  
- Explore **deep learning**-based collaborative filtering methods (e.g., autoencoders)

---

## 👤 Author

**Rohit Shivhare**  
[LinkedIn](https://www.linkedin.com/in/rohit-shivhare-a857a4233/)  
*MSc Data Science – Brunel University, London*
