![yamdb_workflow](https://github.com/Rybakov-Ilay/yamdb_final/workflows/yamdb_workflow/badge.svg)

# API_YaMDb
___

The YaMDb project collects user reviews (Title). 
The works are divided into categories: "Books", "Films", "Music". 
The list of categories (Category) can be expanded 
(for example, you can add the category "Fine Arts" or "Jewelry")

## Getting Started
___
These instructions will get you a copy of the project 
up and running on your local machine for development
and testing purposes. See deployment for notes on how
to deploy the project on a live system.

### Prerequisites

Clone the repository from github.

`https://github.com/Rybakov-Ilay/infra_sp2.git`

### Installing

Make sure docker and docker compose are installed. If not, then install.
Installation instructions for different platforms can be found
on the official website https://docs.docker.com/

Open a terminal and run the command from the root folder:

`docker-compose up`

The process of building and launching containers will start.

Login to the web container:

`docker-compose exec web bash`

Make migrations, create a superuser and optionally
load test data from fixtures.json:

```
python manage.py migrate
python manage.py createsuperuser
python manage.py loaddata fixtures.json
```
Exiting the container:

`exit`

Site is working on  http://0.0.0.0:8000/

* At http://0.0.0.0:8000/api/v1/ the first version of the api is available 

* At http://0.0.0.0:8000/redoc/ there is 
documentation for working with API_YaMDb.

* At http://0.0.0.0:8000/redoc/ site admin panel available 

The `.env` file contains predefined database connection settings.
It is better to change them from the default settings.

## Built With
___

* [Django](https://www.djangoproject.com/)
* [Django Rest Framework](https://www.django-rest-framework.org/)
* [PostgreSQL](https://www.postgresql.org/)
* [Docker](https://www.docker.com/)

## Authors
___

* [Rybakov Ilya](https://github.com/Rybakov-Ilay)

## License
___
This project is licensed under the MIT 
License - see the LICENSE.md file for details

Language: ![https://img.shields.io/badge/Python-3.6.9-blue](https://img.shields.io/badge/Python-3.6.9-blue)


