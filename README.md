# Chatbot Intent Recognition using Google Vertex AI

## Project Overview
This project aims to build and deploy a chatbot intent recognition model using Google Vertex AI. The model is trained on a dataset of customer queries and intents, and is deployed to predict the intent of new customer queries.

## Dataset
The dataset used for training the model is sourced from Kaggle and contains various customer queries and their corresponding intents.

## Project Structure
- `/data`: Contains the dataset.
- `/notebooks`: Jupyter notebooks for data exploration and model training.
- `/scripts`: Python scripts for data preprocessing, model training, and deployment.

## Steps Followed
1. **Data Preprocessing**: Cleaned and preprocessed the data to remove duplicates and ensure proper labeling.
2. **Model Training**: Trained a text classification model using Google Vertex AI AutoML.
3. **Model Evaluation**: Evaluated the model using precision, recall, and F1 score.
4. **Model Deployment**: Deployed the trained model on Google Vertex AI.

## Model Evaluation
| Metric          | Value    |
|-----------------|----------|
| Precision       | 99.9%    |
| Recall          | 99.9%    |
| F1 Score        | 0.9986251|
| Total Items     | 21,513   |
| Training Items  | 17,264   |
| Validation Items| 2,067    |
| Test Items      | 2,182    |

## Visuals
### Precision-Recall Curve
![Precision-Recall Curve]<img width="477" alt="Precision_Recall" src="https://github.com/rdc2697/Chatbot-Intent-Recognition-using-Google-Vertex-AI/assets/40556517/95d46288-fdba-4617-b9ed-f04604ddd866">


### Confusion Matrix
![Confusion Matrix](path/to/Confusion_Matrix.png)

## How to Use the Model
1. **Make Predictions**: Use the deployed model endpoint to make predictions on new customer queries.
2. **API Calls**: Example script for making API calls to the deployed model.

## Credits
This project is developed by Rishabh Dev Chawla.
