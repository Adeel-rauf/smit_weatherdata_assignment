This project uses machine learning to classify weather conditions based on different environmental factors such as temperature, humidity, wind speed, visibility, and air pressure. The main goal is to predict the type of weather using data provided in a CSV file.

## Methods Used
The following methods and tools are used in this project:
- train_test_split  
- ColumnTransformer  
- SimpleImputer  
- OneHotEncoder  
- MinMaxScaler  
- SelectKBest (chi2)  
- DecisionTreeClassifier  
- Pipeline and make_pipeline  

## How It Works
The dataset is first cleaned and processed.  
Missing values are filled using SimpleImputer.  
Categorical values like hour and month are converted into numeric form using OneHotEncoder.  
All numeric features are scaled between 0 and 1 using MinMaxScaler so that chi2 can be applied safely.  
Important features are selected using SelectKBest with chi2, and a Decision Tree model is trained to classify the weather type.

## Output
After training, the model predicts the weather category such as:
- Clear  
- Cloudy  
- Fog  
- Rain  
- Snow or Ice  
- Thunderstorm  
- Other  

The accuracy and performance are printed after testing the model.

## Tools
- Python  
- Pandas  
- Scikit-learn  
- Jupyter Notebook
