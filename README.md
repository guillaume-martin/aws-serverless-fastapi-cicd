# aws-serverless-fastapi-cicd
Learning how to deploy a FastAPI application to AWS Lambda

[FastAPI AWS Lambda Deployment with GitHub Actions Pipeline](https://www.youtube.com/watch?v=UauMQGqaxGo)


# Create application
- Create virtual environment 
```sh
python -m virtualenv venv
source venv/bin/activate
```
- Install FastAPI and Uvicorn
```sh
pip install fastapi uvicorn
```
- Create `api/main.py`
- Start server
```sh
uvicorn api.main:app --reload
```
- Install pytest
```sh
pip install pytest
```
- Create tests/test_core.py


# GitHub Actions - CI/CD Pipeline
- Create `.github/workflows` directory
- Create `main.yml` file


# Set up AWS
## Create an S3 bucket


## Create a Lambda function
- Create new function
- Go to Runtime settings
- Change Handler to `main.handler`
- Install mangum `pip install mangum`
- Add handler to `main.py`

## Create new pipeline for deployment
- Get new access key from AWS
    - My security credentials -> Access Keys -> Create New Access Key
- Go to gihub
- repository -> settings -> secrets -> New repository secret
    - Set name: AWS_SECRET_ACCESS_KEY
    - Paste value

