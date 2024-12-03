# Project Title: Predicting Vehicle Insurance Adoption - A Cross-Sell Model

## Description:
This project aims to predict whether health insurance policyholders are likely to purchase vehicle insurance using a machine learning classification model. The model uses boosting techniques for predictions and is deployed using FastAPI and Streamlit on both Google Cloud Platform (GCP) and AWS.

## Features:
- Machine learning classification model using boosting techniques.
- FastAPI application for model deployment on GCP and AWS.
- Streamlit app for easy user interface and interaction.
- Docker images for AWS deployment.

## Project Structure:

├── fastapi_aws/ # FastAPI application for AWS │ └── [FastAPI files] ├── fastapi/ # FastAPI application for GCP │ └── [FastAPI files] ├── web_app_aws/ # Streamlit application for AWS │ └── [Streamlit files] ├── web_app/ # Streamlit application for GCP │ └── [Streamlit files] ├── cross-sell-prediction/ # Model PKL file │ └── [Model PKL file] ├── links.md # Links for FastAPI & Streamlit └── README.md # Project documentation

## Requirements:
To run the project, you'll need the following:
- Python 3.x
- FastAPI
- Streamlit
- Docker (for AWS)
- Google Cloud SDK (for GCP)
- Other dependencies listed in the `requirements.txt`

## Installation:
Clone the repository:
```bash
git clone https://github.com/Gayathrigopi98/cross-sell-model.git

## How to Run:
For FastAPI  : uvicorn model_app:app --reload
For Streamlit: streamlit run .\webview.py

## For AWS Deployment (using Docker)[Build and run the Docker containers for FastAPI and Streamlit]
docker build -t fastapi-aws .
docker run -p 8000:8000 fastapi-aws

Links:
### GCP – GitHub Links
- [FastAPI Docs](https://cross-sell-model-fastapi-46604026246.us-central1.run.app/docs#/default/predict_predict_post)
- [Streamlit App](https://cross-sell-model-webapp-46604026246.us-central1.run.app)

### AWS – Docker Links
- [FastAPI Docs](https://container-service-1.m6kb1avhqx16c.ap-south-1.cs.amazonlightsail.com/docs#/default/predict_predict_post)
- [Streamlit App](https://container-service-2.m6kb1avhqx16c.ap-south-1.cs.amazonlightsail.com/)

### Docker Images
- FastAPI: `gayathri1708/fastapi-aws:1.0`
- Streamlit: `gayathri1708/streamlit-aws:1.0`

  
Model Evaluation:
ROC-AUC Score: 80.01

