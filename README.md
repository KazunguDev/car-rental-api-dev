# CAR HIRE/RENTALS JSON API WITH RAILS 6

A RESTFUL API built with Ruby on Rails. It uses JWT to implement Authentication & Authorization.
In this project, I built a fullstack application where users can access cars and it's featured amongst the least of cars available for hire. 




## Built With

- Ruby v2.7.2
- Ruby on Rails v6.0.3.2
- RSpec-Rails for testing


## Current API Endpoints

The API will expose the following RESTful endpoints.
### BaseUrl: {Host-URL}/api/v1

| Endpoint                | Functionality                |
|-------------------------|------------------------------|
| POST /register          | Signup                       |
| POST /login             | Login                        |
| GET /users              | List all users               |
| GET /cars               | List all cars                |
| POST /cars              | Add a new car                |
| DELETE /cars/:id        | Delete a car                 |
| PUT /cars/:id           | Update a car                 |
| DELETE /user/:id        | Delete a user                |
| PUT /user/:id           | Update a user                |
| POST /favourites        | Add favourite car            |
| GET /favourites         | Get user favourite cars      |

## API Documentation
[Car Rentals API](https://documenter.getpostman.com/view/171080/TW6tKpYs)
## Getting Started

To get a local copy up and running follow these simple example steps.

### Prerequisites

Ruby: 2.6.5
Rails: 6.0.3.2
Postgres: >=9.5

### Setup

~~~bash

$ cd car-rental-api
~~~

Install gems with:

```
bundle install
```

Setup database with:

> make sure you have postgress sql installed and running on your system

```
   rails db:create
   rails db:migrate
   rails db:seed
```

### Usage

Start server with:

```
    rails server -p 3001
```

Open `http://localhost:3001/` in your browser.

### Deploy to a live server

Deploying to a live server like Heroku is easy, make sure you have the necessary credentials setup on your local machine

```bash
heroku create
heroku rename app-new-name
git push heroku $BRANCH_NAME:master 
```
if you are already in master branch no need to add $BRANCH_NAME, just use `git push heroku master`

```bash
heroku run rails db:migrate
heroku run rails db:seed
heroku open
```

Enjoy your newly deployed rails API


### Run tests

```
    rpsec 
```




