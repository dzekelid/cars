{
  "info": {
    "name": "Expedia Search",
    "_postman_id": "ad87c393-7d06-4853-8333-47e4c53b5bea",
    "description": "Mobile API Cars",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "travel",
      "item": [
        {
          "id": "8237d1cf-d1bb-424f-a0b6-c5577b2ab6ec",
          "name": "cars-search",
          "request": {
            "url": "http://apim.expedia.com/x/m/api/cars/search/location?dropOffTime=%7B%7D&pickupLocation.lat=%7B%7D&pickupLocation.lon=%7B%7D&pickupTime=%7B%7D&searchRadius=%7B%7D&vendorCode=%7B%7D",
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
              "id": "8bb142e4-683d-461e-8540-85aec2d0aa83"
            }
          ]
        }
      ]
    }
  ]
}