{
  "info": {
    "name": "Expedia Search",
    "_postman_id": "75b87ce3-3032-40a6-9372-2b13a00f00cc",
    "description": "Mobile API Cars",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "travel",
      "item": [
        {
          "id": "7328de83-a39f-4f6b-8624-55f39e54cd3b",
          "name": "cars-search",
          "request": {
            "url": "http://apim.expedia.com/x/m/api/cars/search/airport?airportCode=%7B%7D&dropOffTime=%7B%7D&pickupTime=%7B%7D&vendorCode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Mobile API Cars"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00daca72-cc84-4eb4-adda-51f1c2628435"
            }
          ]
        }
      ]
    }
  ]
}