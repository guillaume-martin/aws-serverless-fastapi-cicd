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

