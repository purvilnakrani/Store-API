# STORE API

This store api created to get all awailable items from the store database. Ex- A store having woodnen chair, dining table, bench etc with details of company name , featured, rating, price.


## Installation

If you want to work on this project , clone this repo

```bash
git clone "https://github.com/purvilnakrani/Store-API.git"

```

Open this project on your local IDE and in the terminal do this commands one by one

 ```
 npm install
 npm run start
```

Before running code do not forget to change database connection url, To get that url go to mongodb atlas cluster -> connect -> driver
Ex:- `MONGODBURI: mongodb+srv://<user_name>:<password>@mongodb_connection_string/database_name`


## API Reference

Base URL
```https
localhost:3000/
```

- get list of all producta from store
```http
  GET /products
```
- get list static producta from store
```http
  GET /products/static
```
- Url query searching
```http
  GET /products?name=bench&featuted=true
```
- Url query searching (page)
```http
  GET /products?featuted=false&page=2
```
- Url query searching (enum)
```http
  GET /products?featuted=false&company=ikea
```
- Url query searching (Numeric filters)
- ```http
  GET /products?numericFilters=price<100,rating>=4
```




## Tech Stack


**Server:** Node, Express

**database:** MongoDB

