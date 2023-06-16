# APIs authentication and Recipe Data from BantuMasak

#### _The Last Markdown Editor, Ever_

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

BantuMasak is an Android application with a main feature designed to assist housewives in planning meals for multiple days. The application provides a wide range of recipes that can be added to the meal plan section, complete with ingredients and step-by-step instructions for preparing the dishes.

- See the two BantuMasak APIs above
- Cloud Computing Documentation from BantuMasak Team
- ✨Thank You

## Features

### [JsonWebToke API](https://github.com/MunzirT/spncRecipeAPI/tree/main/jwtAPI)
- Provides a user REGISTRATION endpoint
- Provides a user LOGIN endpoint
- Provides a user token VALIDATION endpoint
- Provides a user LOGOUT endpoint, as well as DELETES already registered tokens

### [Recipe API](https://github.com/MunzirT/spncRecipeAPI/tree/main/theMealsDB-API)
- Shows all owned recipes (taken from [Spoonacular](https://spoonacular.com) - Open Source API for FOOD Recipes)
- Provides an endpoint so that users can SEARCH for RECIPES BASED ON THE INGRESIENTS they have.
- Provides an endpoint for ADMIN to ADD recipes.
- Provides an endpoint to be able to VIEW RECIPES BY ID.
- Provides an endpoint for ADMIN to DELETE recipes.


## Tech

BantuMasak uses a number of open source projects to work properly:

- [Visual Studio Code](https://code.visualstudio.com/) - awesome open source text editor
- [Postman](https://www.postman.com/) - API development tool that allows to test, manage and document APIs.
- [axios](https://axios-http.com/docs/intro) - great UI boilerplate for modern web apps
- [node.js](https://nodejs.org/) - evented I/O for the backend
- [Express](https://expressjs.com/) - fast node.js network app framework

And of course BantuMasak itself is open source

## Cloud Computing Documentation

## API Auth

#### Get the MAIN page

```http
  GET http://localhost:3000/
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| ``        | ``       | **Required**. Main Page "Hello, Word" |

#### Post the Register form

```http
  POST http://localhost:3000/api/auth/register
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `username`      | `string` | **Required**. username of acount to fetch |
| `password`      | `string` | **Required**. password of item to fetch |

#### Post the Login form

```http
  POST http://localhost:3000/api/auth/login
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `username`      | `string` | **Required**. username of acount to fetch |
| `password`      | `string` | **Required**. password of item to fetch |

#### Post the Logout Page

```http
  POST http://localhost:3000/api/auth/logout
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `Token`      | `Bearer` | **Required**. Token from Loing of acount to fetch |


## API Recipes

#### Get All Recipes

```http
  GET http://localhost:3000/recipes
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `...`      | `...`    | GET ALL ITEM |

#### Get Recipes by ID

```http
  POST http://localhost:3000/recipes/{id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `id` | **Required**. Token from Loing of acount to fetch |

#### Get Recipes by Ingredients

```http
  http://localhost:3000/search?
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
|`ingredients`| `string` | **Required**. Token from Loing of acount to fetch |







