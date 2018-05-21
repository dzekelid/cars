{
  "info": {
    "name": "Expedia Search",
    "_postman_id": "870f08c4-71d5-4dec-8305-a1e2d0b2d8c0",
    "description": "Mobile API Cars",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "travel",
      "item": [
        {
          "id": "0d652236-d999-4cb7-ae5a-d6550066407f",
          "name": "cars-search",
          "request": {
            "url": "http://apim.expedia.com/x/m/api/cars/search?destinationAirportCode=%7B%7D&dropOffLocation.lat=%7B%7D&dropOffLocation.lon=%7B%7D&dropOffTime=%7B%7D&originAirportCode=%7B%7D&pickupLocation.lat=%7B%7D&pickupLocation.lon=%7B%7D&pickupTime=%7B%7D&searchRadius=%7B%7D&vendorCode=%7B%7D",
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
              "id": "33e3bbe6-60f8-430e-8e07-1461f80070b9"
            }
          ]
        }
      ]
    }
  ]
}