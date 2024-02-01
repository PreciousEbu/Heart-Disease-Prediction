# Heart-Disease-Prediction

### Overview

According to the World Health Organization (WHO), With 17.9 million deaths per year, cardiovascular diseases (CVDs) are the leading cause of death worldwide. Coronary heart disease, cerebrovascular disease, rheumatic heart disease, and other illnesses are among the category of heart and blood vessel disorders known as CVDs. Heart attacks and strokes account for more than four out of every five CVD deaths, and one third of these deaths happen before the age of 70.

Unhealthy eating, inactivity, usage of tobacco products, and abusing alcohol are the main behavioral risk factors for heart disease and stroke. Individuals may experience elevated blood pressure, elevated blood glucose, elevated blood lipids, as well as overweight and obesity as a result of these risk factors. These "intermediate risk variables" can be assessed in primary care settings and point to an elevated risk of consequences like heart attack, stroke, and heart failure.
Premature deaths can be avoided by identifying those who are most at risk for CVDs and ensuring they receive the proper care and on time. Thus, the need to predict the case of heart disease correctly is essential.

#### Problem and Approach

The problem this data is used to solve is a classification problem and the approach used was Machine Learning.

#### Data
The dataset used for this project was downloaded from Kaggle. The dataset contains 253680 observations and 22 variables, that is, 1 response variable (HeartDiseasorAttack) and 21 other predictor variables some of which are, BMI, high cholesterol, Physical activity, Mental health, Diabetes, Stroke etc. The dataset was highly imbalanced with 90% of cases occurring as no heart disease or attack.

#### Findings and Results

-	**Data Processing**: Not much was done on missing values because the data came clean. Nonetheless, data type conversions were carried out.
  
-	**Data Visualization**: Graphs were plotted to get visible insights on the different variables. Histograms were plotted for each feature with the representation of the cases of heart disease or not. Box plots were also plotted to visualized outliers. Relationships between variables were also visualized using a heatmap and correlation plot.
  
-	**Exploratory Data Analysis (EDA)**: The data was explored for further insights. Outliers were detected and treated by replacing with the column means. Statistical analysis were performed to test for relationships between variables using chi-square test of independence. The response variable “Heartdiseaseorattack” had a statistical significant relationship with all predictor variables. From our results, 90.58% of cases did not have heart disease or attack while 9.42% of cases had heart disease or attack. Feature importance was done using boruta to determine the most important variables. 3 features (high BP, high cholesterol and smoker) were deemed unimportant and dropped.

####	Machine Learning
- Data Science through Machine learning has helped provide ways to build predictive models that assist healthcare and other industries. With the help of machine learning, we were able to use algorithms to predict the cases of heart disease or attack or not. Various machine learning models were built to get the best performing models.
- Since the problem is a classification problem, logistic regression was used to build models. The data was first up-sampled using ROSE to balance the classes of the target variable. The ROSE data was fit through random forest algorithm and logistic regression with interaction effect. To get the best performing model. Due to the nature of the data and the high level of imbalance between the classes, the evaluation metrics used were specificity, sensitivity, F1 and Recall. Cross validation was also done using the generalized linear model to improve the model performance. 
- The final model had an accuracy of 75% with Sensitivity and Specificity of 76% and 75% respectively.
