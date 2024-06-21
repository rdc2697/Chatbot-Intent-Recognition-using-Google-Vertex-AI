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

## Model Training
The model was trained using Google Vertex AI's AutoML for text classification. Key steps include:
1. Importing the cleaned dataset.
2. Training the model using Vertex AI.
3. Evaluating the model's performance.

## Deployment
The trained model was deployed to an endpoint on Google Vertex AI, allowing it to serve online predictions.

## Usage
To use the deployed model, send a POST request with the input text to the endpoint. Example input and output:

**Input: {
"instances": [
{"content": "I'm unhappy with the service and want my money back."}
]
}**

**Output:
{
"predictions": [
{
"displayName": "complaint",
"confidence": 0.945
}
]
}**

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
<img width="477" alt="Precision_Recall" src="https://github.com/rdc2697/Chatbot-Intent-Recognition-using-Google-Vertex-AI/assets/40556517/95d46288-fdba-4617-b9ed-f04604ddd866">


### Confusion Matrix with Item Counts

<img width="502" alt="confusion_matrix" src="https://github.com/rdc2697/Chatbot-Intent-Recognition-using-Google-Vertex-AI/assets/40556517/c0587042-f451-4a59-9d21-08bebea12962">
<img width="479" alt="confusion_matrix_item_counts" src="https://github.com/rdc2697/Chatbot-Intent-Recognition-using-Google-Vertex-AI/assets/40556517/d02a09ad-362a-4e0b-b19c-6da54cdc1b4f">


## How to Use the Model
1. **Make Predictions**: Use the deployed model endpoint to make predictions on new customer queries.
2. **API Calls**: Example script for making API calls to the deployed model.

## Credits
This project is developed by Rishabh Dev Chawla.
