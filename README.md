# SageMaker-ML-Workflows: Automated Tuning, A/B Testing & Human-in-the-Loop

This GitHub repository contains Python notebooks that demonstrate how to use Amazon SageMaker to build, train, and deploy machine learning models. The repository focuses on three key workflows: Automated Hyperparameter Tuning, A/B Testing, and Human-in-the-Loop Pipelines using Amazon Augmented AI (A2I).

## Table of Contents

1. [Automated Hyperparameter Tuning](#automated-hyperparameter-tuning)
2. [A/B Testing, Traffic Shifting, and Autoscaling](#ab-testing-traffic-shifting-and-autoscaling)
3. [Data Labeling and Human-in-the-Loop Pipelines with Amazon Augmented AI (A2I)](#data-labeling-and-human-in-the-loop-pipelines-with-amazon-augmented-ai-a2i)
4. [Installation & Setup](#installation--setup)
5. [Contributing](#contributing)

## Automated Hyperparameter Tuning

### Introduction
This notebook demonstrates how to use Amazon SageMaker's Automated Hyperparameter Tuning feature to optimize a BERT-based NLP classifier. The model classifies customer feedback into positive, neutral, or negative sentiments.

#### Notebook Contents:
- Configure dataset and Hyperparameter Tuning Job
  - Configure dataset
  - Configure Hyperparameter Tuning Job
  - Set up evaluation metrics
- Run tuning job
  - Set up the RoBERTa and PyTorch script to run on SageMaker
  - Launch the Hyperparameter Tuning Job
  - Check Tuning Job status
- Evaluate the results
  - Show the best candidate
  - Evaluate the best candidate
  - Inspect the processed output data

[View Notebook](#)

## A/B Testing, Traffic Shifting, and Autoscaling

### Introduction
This notebook explains how to set up an endpoint with multiple variants in Amazon SageMaker, perform A/B testing, and finally configure autoscaling.

#### Notebook Contents:
- Create an endpoint with multiple variants
  - Construct Docker Image URI
  - Create Amazon SageMaker Models
  - Set up Amazon SageMaker production variants
  - Configure and create endpoint
- Test model
  - Test the model on a few sample strings
  - Generate traffic and review the endpoint performance metrics
- Shift the traffic to one variant and review the endpoint performance metrics
- Configure one variant to autoscale

[View Notebook](#)

## Data Labeling and Human-in-the-Loop Pipelines with Amazon Augmented AI (A2I)

### Introduction
Learn how to use Amazon A2I to create your human review workflows for machine learning models. This notebook covers creating a human workforce, Human Task UI, and defining the human review workflow.

#### Notebook Contents:
- Set up Amazon Cognito user pool and define human workforce
  - Create Amazon Cognito user pool
  - Create Amazon Cognito user pool client
  - Create Amazon Cognito user pool domain and group
  - Create workforce and workteam
  - Create an Amazon Cognito user and add the user to the group
- Create Human Task UI
- Define human review workflow
- Start human loop with custom ML model
  - Deploy a custom model
  - Start the human loop
  - Check status of the human loop
  - Complete the human loop tasks
  - Verify that the human loops were completed by the workforce
  - View human labels and prepare the data for re-training

[View Notebook](#)

## Installation & Setup

Clone the GitHub repository and install the required Python packages.

```bash
git clone <repository-link>
cd <repository-directory>
pip install -r requirements.txt
```

## Contributing

Feel free to contribute to this project by submitting pull requests or issues.

[Back to Top](#table-of-contents)
```
