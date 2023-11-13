# Name of Project

## Week 7 Large group project

The focus of this app is to practice using the Full Stack we teach, (with auth in place) in a large scale app.

The idea of the app is to xxxx


## The Tech

A Boilerplate is already set up for you with everything you will need to get started. This boilerplate is set up to use:

* [React](https://reactjs.org/docs/getting-started.html)
* [ReactQuery](https://tanstack.com/query/v4/docs/react/overview) 
* [Express](https://expressjs.com/en/api.html)
* [Knex.js](https://knexjs.org/)
* [Sass](https://sass-lang.com/)

The migration and seeds for the users table, and all login functionality is already set up!

The mobile responsiveness is also being handled by some neat JS and Sass classes, be sure to incorporate that view in your project goals!

## User Stories

### MVP

As a non-registered user:
* I want to xxx
* I want to xxx
* I want to xxx
* I want to xxx


As a registered user:
* I want to xxx
* I want to xxx
* I want to xxx
* I want to xxx

### Stretch

As a registered user:
* I want to xxx
* I want to xxx
* I want to xxx
* I want to xxx


---

## Views (Client Side)

| name | purpose |
| --- | --- |
| Login | View for user to enter their login credentials |
| Register | View for user to sign up |
| Home | Welcome users and links to app|
| View Name | View Description |




## API (Client - Server)

| Method | Endpoint | Protected | Usage | Response |
| --- | --- | --- | --- | --- |
| Post | /api/v1/auth/login | Yes | Log In a User | The Users JWT Token |
| Post | /api/v1/auth/register | Yes | Register a User | The Users JWT Token |
| Get | /api/v1/data | No | Get all data | Array of Objects (object = a data) |
| Post | /api/v1/data | Yes | Add data to the db | 201 status code |

## DB (Server Side)

Write and display the structure of the data

### Table 1 

| Column Name | Data Type | Purpose |
| --- | --- | --- |
| id | integer | Unique identifier for each review |
| name | string | Name of thing |
| text | text | data's text |
| date | date | when created|

### Table 2 

| Column Name | Data Type | Purpose |
| --- | --- | --- |
| id | integer | Unique identifier for each review |
| name | string | Name of thing |
| text | text | data's text |
| date | date | when created|

### Saved Reviews (Many to Many / join table)

| Column Name | Data Type | Purpose |
| --- | --- | --- |
| id | integer | Unique identifier |
| table_1_id | integer | ...|
| table_2_id | integer | ... |

## Authentication

Authentication is already set up in this project using the node module [authenticare](https://www.npmjs.com/package/authenticare). Users are currently able to login, logout, and register and all user information will be stored in a table in our database.

If you wish to dive deeper on authenticare, docs are avalable [here](https://github.com/enspiral-dev-academy/authenticare/tree/main/docs). Of particular note are `getEncodedToken` and `getTokenDecoder` as they deal with how you add a token to your request and secure server routes respectively.


---

## Setup

Run the following commands in your terminal:

```sh
npm install
npm run knex migrate:latest
npm run knex seed:run
cp .env.example .env
```

To run in development:
```sh
npm run dev
```

To run in production:
```sh
npm start
```


## Deployment

Follow the [Dokku Guide]() to deploy your site.
