#  Iris Flower Classification

This is a basic machine learning project that uses the classic **Iris dataset** to explore classification techniques, the power of visualization, and the impact of thoughtful feature selection in building efficient models.

---

##  Objective

- Explore feature relationships visually
- Understand the structure of the Iris dataset
- Highlight how thoughtful feature pairing can simplify modeling
- Build an efficient classification model using clean preprocessing and pipeline methods

---

##  Dataset

- **Source**: [Kaggle - Iris Dataset](https://www.kaggle.com/datasets/uciml/iris)
- **Classes**: Setosa, Versicolor, Virginica
- **Features** (all in cm):
  - SepalLength
  - SepalWidth
  - PetalLength
  - PetalWidth

---

##  Key Observations

- The dataset shows **strong linear separability**, especially between **PetalLength** and **PetalWidth**
- Simple scatter plots reveal clear clustering patterns
- A basic **linear classifier like SVM** is sufficient for high accuracy on this dataset

---

## ⚙ Implementation Details

###  Libraries Used
- `pandas`, `numpy` – for data handling
- `matplotlib`, `seaborn` – for data visualization
- `scikit-learn` – for model building and evaluation

###  Steps Followed
1. Data cleaning and basic exploration
2. Label encoding using `OrdinalEncoder`
3. Feature visualization using `matplotlib.pyplot.scatter`
4. Stratified train-test split to preserve class distribution
5. Model training:
   - **Linear SVM** as the primary model
   - **RandomForestClassifier** used for comparison
6. Hyperparameter tuning using `RandomizedSearchCV` based on **F1-score**

---

##  Results

- Developed a **simple yet highly effective classification model**
- Achieved strong performance primarily due to the **linearly separable nature of the dataset**
- Reinforced the value of **visual data inspection** in guiding model choice

---
