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
To showcase your work on the dataset preparation, training, and deployment of the chatbot model using Google Vertex AI in your GitHub repository, you should include the following:

Jupyter Notebook: Upload the Jupyter Notebook where you performed data cleaning and preparation. This notebook should include all the steps you took to clean the dataset and any exploratory data analysis (EDA) you performed. Name this file appropriately, e.g., Data_Cleaning_and_Preparation.ipynb.

README File: Update the README file to provide an overview of the project, including:

Introduction: A brief description of the project and its goals.
Dataset: Information about the dataset used, including where it was sourced from and how it was cleaned (link to the Jupyter Notebook).
Model Training: Explain how the model was trained using Google Vertex AI, including steps for creating the dataset, training the model, and evaluating it.
Deployment: Describe the deployment process of the trained model to an endpoint on Google Vertex AI.
Usage: Instructions on how to use the deployed model, including example input and output.
Files: A list of files included in the repository with descriptions of their contents.
Script for Vertex AI: If you have any Python scripts or commands that were used to interact with Google Vertex AI, include those in a separate folder, e.g., vertex_ai_scripts.

Screenshots and Visuals: Add screenshots of the key steps in Vertex AI (e.g., dataset import, model training, evaluation metrics, and deployment). Place these images in a folder named images and link to them in the README file.

Here is an example structure for your repository:

arduino
Copy code
Chatbot-Intent-Recognition-using-Google-Vertex-AI/
│
├── data/
│   └── ultracleaned_chatbot_dataset.csv
│
├── vertex_ai_scripts/
│   └── vertex_ai_training.py (example script if applicable)
│
├── images/
│   └── data_import.png
│   └── model_training.png
│   └── evaluation_metrics.png
│   └── deployment.png
│
├── Data_Cleaning_and_Preparation.ipynb
├── LICENSE
├── README.md
README.md Example Content
markdown
Copy code
# Chatbot Intent Recognition using Google Vertex AI

## Introduction
This project demonstrates the complete workflow for building, training, and deploying a chatbot intent recognition model using Google Vertex AI.

## Dataset
The dataset used for this project contains customer utterances and their corresponding intents. The data was sourced from [Kaggle](https://www.kaggle.com/datasets/niraliivaghani/chatbot-dataset/data). The dataset was cleaned and prepared using a Jupyter Notebook, which can be found [here](data/Data_Cleaning_and_Preparation.ipynb).

## Model Training
The model was trained using Google Vertex AI's AutoML for text classification. Key steps include:
1. Importing the cleaned dataset.
2. Training the model using Vertex AI.
3. Evaluating the model's performance.

## Deployment
The trained model was deployed to an endpoint on Google Vertex AI, allowing it to serve online predictions. [Screenshots](images/deployment.png) of the deployment process are provided.

## Usage
To use the deployed model, send a POST request with the input text to the endpoint. Example input and output:

**Input:
{
"instances": [
{"content": "I'm unhappy with the service and want my money back."}
]
}**

makefile
Copy code

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
