# CDK Python Project for API Gateway, Lambda, and DynamoDB

This is a CDK project that sets up an API Gateway to manage CRUD operations on tasks using AWS Lambda functions integrated with DynamoDB.

## Project Structure
![IMG_20240918_173031](https://github.com/user-attachments/assets/0c5815ec-a537-44cb-8c89-18a7417a8981)


- `task_api_stack.py`: The main CDK stack that defines resources including DynamoDB, Lambda functions, and API Gateway.
- `lambda_resources.py`: Defines Lambda functions for creating, reading, updating, and deleting tasks.
- `dynamodb_resources.py`: Sets up the DynamoDB table to store tasks.
- `cdk.json`: Configures how the CDK toolkit runs your project.
- `.env`: Stores environment variables like AWS account ID and region for the deployment.

## Prerequisites

- Python 3.x
- AWS CDK Toolkit installed globally (`npm install -g aws-cdk`)
- AWS CLI configured with appropriate credentials (`aws configure`)

## Setup Instructions

1. Clone the repository and navigate into the project directory:
      ```bash
         git clone <repository-url>
         cd crud_task_api
2. Install required dependencies:
    ```bash
    pip install -r requirements.txt
3. Set up your .env file:
    ```bash
      CDK_DEFAULT_ACCOUNT=  # Replace with your AWS Account ID
      CDK_DEFAULT_REGION=   # Replace with your preferred AWS region
4. cdk bootstrap 
      ```bash
      cdk bootstrap
          The cdk bootstrap command in AWS CDK initializes the environment in which you will deploy CDK applications. It sets up the necessary resources in your AWS account to support CDK deployments.
5. cdk deploy 
    ``` bash
    cdk deploy 
        The cdk deploy command in AWS CDK is used to deploy your CDK application to your AWS account.
### After cdk deploy :
  You will see something like this 
![IMG_20240918_175142](https://github.com/user-attachments/assets/000c6829-f646-413c-9a31-b080c56751a5)

![IMG_20240918_175247](https://github.com/user-attachments/assets/a01fed9b-170f-49d4-98ea-f7af643fe02e)

![IMG_20240918_175123](https://github.com/user-attachments/assets/d12cc22c-4943-48cb-8362-7b7c3df64e8f)




