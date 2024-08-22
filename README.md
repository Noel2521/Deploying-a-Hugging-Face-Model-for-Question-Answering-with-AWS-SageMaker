## Deploying a Hugging Face Model for Question Answering with AWS SageMaker

### This repository demonstrates how to deploy a Hugging Face question-answering model on AWS SageMaker. 
### Using the Boto3 and SageMaker SDKs, this project shows how to set up a scalable inference endpoint for natural language processing tasks.

## Overview
### This project uses AWS SageMaker to deploy a Hugging Face model designed for question answering. The model selected for this example is distilbert-base-uncased-distilled-squad, which is a smaller, faster, and more efficient version of BERT fine-tuned on the SQuAD dataset.

### The deployment is achieved using the following technologies:

- SageMaker: An AWS service for building, training, and deploying machine learning models.
- Boto3: The AWS SDK for Python, which allows for the management of AWS services like IAM roles.
- Hugging Face Transformers: A library for state-of-the-art NLP models.

## Prerequisites
### Before you begin, ensure you have the following:

- AWS Account: An AWS account with the necessary permissions to create and manage SageMaker resources.
- AWS CLI: The AWS CLI configured on your machine.
- Python 3.x: Python installed along with pip for package management.
- SageMaker SDK: Install the SageMaker Python SDK using pip install sagemaker.
- Boto3 SDK: Install Boto3 using pip install boto3.

## Code Explanation
### The provided script does the following:

## Session and Role Management:
- Creates a SageMaker session.
- Determines the default S3 bucket for SageMaker.
- Retrieves or creates the IAM role needed for SageMaker execution.

## Model Configuration:
- Specifies the Hugging Face model and task.
- Sets up the environment with the appropriate versions of Transformers, PyTorch, and Python.

## Model Deployment:
- Deploys the model to a SageMaker endpoint using the specified instance type.

## Prediction:
- Demonstrates how to make predictions using the deployed model with example inputs.
- Running the Example

- After deploying the model, you can run the example prediction code to test the endpoint. The sample requests demonstrate how to ask questions related to provided contexts and receive answers from the model.
