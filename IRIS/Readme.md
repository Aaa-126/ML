# Iris Flower Classification

## Objective

This is a machine learning classification project using the classic **Iris dataset**. The aim is to explore how visualization, data pairing, and simple preprocessing can lead to an efficient and interpretable model.

Through this project, we aim to:
- Visually explore feature relationships.
- Understand the structure and properties of the Iris dataset.
- Highlight how thoughtful feature selection and pairing simplify model building.
- Build a classification model using clean preprocessing and modern ML pipeline techniques.

## Dataset

- Source: Downloaded from Kaggle
- Classes: Setosa, Versicolor, Virginica
- Features:
  - Sepal Length (cm)
  - Sepal Width (cm)
  - Petal Length (cm)
  - Petal Width (cm)

## Key Observations

1. The dataset exhibits strong linear separability, especially between Petal Length and Petal Width.
2. Simple scatter plots reveal clear clustering patterns.
3. A simple linear classifier (e.g., Support Vector Machine) is highly effective for this dataset.

## Implementation Details

### Libraries Used
- `pandas`, `numpy`: For data handling
- `matplotlib`, `seaborn`: For data visualization
- `scikit-learn`: For model building and evaluation

### Steps Followed
1. Data cleaning and basic exploration
2. Label encoding using `OrdinalEncoder`
3. Feature visualization using scatter plots
4. Stratified train-test split
5. Trained:
   - A simple linear SVM model
   - A complex model (RandomForestClassifier) for comparison
6. Model tuning using `RandomizedSearchCV` based on F1 score

## Results

- Developed a good simple efficient classification model due to linear separability of dataset.
- Emphasis on how data visualization informs model choice.

