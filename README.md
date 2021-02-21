# Node Express Mongo Docker Example

This is a sample application demonstrating how to containerize an Node.js express RESTful application that integrates with MongoDB 

## Running the application

1. Clone the repo
2. Spin up containers: `docker-compose up -d`


## Access REST API

1. POST http://localhost:3000/item

   Content-Type: application/json

   {
        "name": "Grapes",
        "quantity": 3
   }



2. GET http://localhost:3000/items

    output:
          [
    {
        "id": "60319e66168092461ba41928",
        "name": "Grapes",
        "quantity": 3
    }
]

3. PUT  http://localhost:3000/item/{id}/quantity/5