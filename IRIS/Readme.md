This is a basic classification project Using iris dataset.
This is to explore several utilitiies and how the good data peering 
helps in building a model that is effiecient and simple.

The iris dataset used is standard one and if you look carefully at the 
plots you can clearly see that if data is linearly separated would provide a 
good result.



Iris Flower classification

1.Objective -

	This is a basic machine learning project that uses the classic Iris-dataset to 	explore classification techniques and the power of visualization and proper data pairing in model building.

	1.Explore feature relationships visually.
	2.Understand the structure of the Iris dataset.
	3.Highlight how thoughtful feature pairing can simplify modeling.
	4.Build an efficient classification model using clean preprocessing and pipeline methods.


2.Dataset -
	Source - downloaded from kaggle
	Classes - Setosa, Versicolor, Virginica
	Features - SepalLength, SepalWidth, PetalLength, PetalLength in cm
	

3. Key Observation -
	1. The dataset shows strong linear separability in feature, especially between PetalLength and PetalWidth
	2.Simple visualisation using scatter plots reveals clear clustering patterns.
	3.A simple linear classifier, like svm,  will do a great job.
	
4. Implementation Details-
	a. Libraries Used-
		i. pandas, numpy - data handling
		ii. matplotlib, seaborn - for data visualization
		iii. scikit-learn - for model building, and evaluation
		
	b. Steps -
		i. Data cleaning and basic exploration.
		ii. Label encoding using 'OrdinalEncoder'.
		iii. feature visualization using 'matplotlib.pyplot.scatter'.
		iv. Stratified train-test data splitting.
		v. Trained a simple linear SVM model and a complex model like RandomForestClassifier - for comparison purpose only	
		vi. model Tuning using RandomSearchCV based on f1 score
		
5. Results- 
	-Developed a good simple efficient classification model due to linear separability of dataset.
	
	- Emphasis on how data visualization informs model choice.
		
	