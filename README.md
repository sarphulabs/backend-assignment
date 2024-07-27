# Take Home Assignment 

This take-home assignment is designed to evaluate your skills in developing APIs using Python, FastAPI, and PostgreSQL. Please ensure that you complete this assignment within 2-3 hours.

## Objective
A simple JWT based auth server that lets user to register, login and fetch user profile. This project uses JWT for authentication (RSA signing method) and a relational database (PostgreSQL) for storing user info.

## Instructions

### 1. Setup the Environment:

- Create a new Python project with a virtual environment.
- Initialize a FastAPI application.
- Set up PostgreSQL database (You can use a local database or a cloud-based service like Heroku)

### 2. Create database schema for user profile
Use following fields: 
name, email, location, about, password

### 3. Develop following endpoints

| Endpoint | Body Fields | Method| Remarks |
|----------|------|--------|--------|
| `api/v1/register-user` | `name`, `email`, `location`, `about`, `password`| POST| Password is saved in encrypted format|
| `/api/v1/auth/login`| `email`, `password` | POST | |
| `/api/v1/auth/refresh-token`| `refresh-token` | POST||
| `api/v1/me`| | GET| Use token in Authorization Header for User Profile|

### 4. Error Handling
Implement proper error handling with proper status codes.

### 5. Documentation
Ensure that your API documentation is accessible at `/docs`

Add a README.md file explaining how to setup and run the project locally.

## Submission
- Create a Github repository and make it public.
- Push your code to the repo.
- Share the link to us.

## Evaluation Criteria
We'll evaluate your code in following criteria: 

- Code Quality
- Functionality
- Error Handling
- Documentation

