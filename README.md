# Insurance Premium Prediction API

A machine learning-based REST API that predicts insurance premium categories based on customer information. The model is served using **FastAPI** and the application is containerized using **Docker**.

## Project Overview

This project provides an API for predicting insurance premium categories using a trained machine learning model.

The API accepts customer information such as age, weight, height, income, smoking status, city, and occupation, and returns the predicted insurance premium category.

## Features

* Machine Learning-based insurance premium prediction
* REST API using FastAPI
* Interactive Swagger API documentation
* Pydantic-based request validation
* Dockerized application
* Docker Hub image
* Modular project structure
* Easy local and containerized deployment

## Technologies Used

* Python
* FastAPI
* Uvicorn
* Scikit-learn
* Pandas
* Pydantic
* Docker

## API Input

The API accepts the following customer information:

* Age
* Weight
* Height
* Income (LPA)
* Smoking Status
* City
* Occupation

The provided information is processed by the trained machine learning model to predict the insurance premium category.

### 1. Clone the Repository

```bash
git clone https://github.com/Rits05/insurance-premium-api.git
```

### 2. Navigate to the Project

```bash
cd insurance-premium-api
```

### 3. Create Virtual Environment

```bash
python -m venv myenv
```

### 4. Activate Virtual Environment

Windows:

```bash
myenv\Scripts\activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the FastAPI Application

```bash
uvicorn app:app --reload
```

The API will run at:

```text
http://127.0.0.1:8000
```

## Swagger API Documentation

After starting the application, open:

```text
http://127.0.0.1:8000/docs
```

Swagger UI allows you to test the API endpoints directly from the browser.

## Run Using Docker

The application is containerized using Docker for easy deployment and portability.

### Build Docker Image

```bash
docker build -t insurance-premium-api .
```

### Run Docker Container

```bash
docker run -p 8000:8000 insurance-premium-api
```

The API can then be accessed at:

```text
http://127.0.0.1:8000
```

Swagger documentation:

```text
http://127.0.0.1:8000/docs
```

## Docker Hub

Docker image repository:

```text
riti05/insurance-premium-api
```

### Tag Docker Image

Replace `tagname` with the desired image tag:

```bash
docker tag insurance-premium-api riti05/insurance-premium-api:tagname
```

### Push Docker Image

```bash
dock
```
