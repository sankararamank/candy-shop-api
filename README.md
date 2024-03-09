# Candy Shop API
Welcome to the Candy Shop API . This repo is a fun project to design, architect and develop an e-commerce backend API in DJango. As some of you may have realised, the name is inspired by 50 Cent's song Candy Shop.

## Setup
Pre-requisites
1. Locally installed python and its dependencies such as venv etc.
2. Locally setup git

Please follow these steps to setup the project.
1. Clone the repo locally.
2. Inside the project directory setup virtualenv for the project using `python -m venv venv`
3. Install python modules using `pip install -r requirements/local.txt`
4. Copy `.env.example` as `.env` and update the `SECRET_KEY` value using known methods. I recommend assigning the string generated [here](https://djecrety.ir/) to `SECRET_KEY` in `.env` file.
5. Test if the server is running using `python manage.py runserver` and open https://localhost:8000 on browser to see the django default page.

## Contribution Guidelines
To contribute please follow the guidelines mentioned in the contribution guidelines [here](docs/contributing.md)

## Though Process
You can find the ideation, design philosophy and other things that was considered while making this project [here](docs/design.md) 
