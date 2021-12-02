# ID checker
##### This is just a project with an example of using flask, Postgres and Docker

The application checks if the ID entered by the user is in the database and returns answer 

- Type ID to the form
- See the answer
- Also you can add you ID if it doesn't exist to the database

## Installation

First fork the repo then do a git clone.

```sh
git clone https://github.com/<yournamehere>/id_checker.git
```
You should also have docker. If you're on linux, you probably also want docker-compose. Last I checked (over a year ago) it did not come with docker by default. For Mac and Windows you get it with the default installation.

Once you have all of that, you should be good. No need to install Postgres or even Python.

build an environment
```sh
docker-compose build
```
start an environment

```sh
docker-compose up -d
```
add a dummy data to database
```sh
docker-compose exec web python manage.py seed_db
```
check if it works by the link:
 [http://localhost:5050/][PlDb]