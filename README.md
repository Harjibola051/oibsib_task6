# oibsib_task6

# Wine Quality Prediction Using Machine Learning
## Project Overview
This project leverages machine learning models to predict wine quality based on chemical properties. Three models—Random Forest, Stochastic Gradient Descent (SGD) Classifier, and Support Vector Classifier (SVC)—were trained and evaluated for performance.

## Dataset
- **Dataset Source:** Wine Quality Dataset (WineQT.xlsx)
- **Target Variable:** Quality (ranges from 3 to 8)
- **Features:** 11 chemical attributes (e.g., alcohol, residual sugar, sulphates, chlorides)
  
## Data Preprocessing
### Handling Outliers

Outliers were detected and handled using the Interquartile Range (IQR) method.

Three strategies were applied:

- Removal of extreme outliers.
- Trimming to replace outliers with boundary values.
- Capping to limit values within the IQR range.
  
## Data Scaling
Standardization using StandardScaler was applied to improve model performance.

## Model Performance
- **Model: 	  Random Forest**
- Accuracy	 69.9%	
- Strengths  	Best overall performance, effective on common classes
- Weaknesses Struggles with rare classes (Quality 3, 4, 8)


- **Model	:  SGD Classifier**			
- Accuracy	 59.7%
- Strengths  Performs well on Quality 5
- Weaknesses Overfitting on specific cases (e.g., Quality 7)


- **Model	:  Support Vector Classifier (SVC)**		
- Accuracy	 65.6%	
- Strengths  Balanced performance 
- Weaknesses  Struggles with extreme quality levels

## Key Insights
- Alcohol and sulphates positively correlate with higher quality wines.
- Volatile acidity and density are inversely related to wine quality.
- Random Forest outperforms other models with 69.9% accuracy.


##  Visual Analysis
- **Correlation Heatmap**

- **Wine Quality Distribution**

- **Boxplots of Key Features**

## Conclusion
Random Forest emerged as the best-performing model, but further improvements can be achieved through feature selection and advanced ensemble techniques.

