{
  "info": {
    "name": "Expedia Cancel Trip",
    "_postman_id": "a6bb5c7f-1ab5-49fc-b2be-9054e5be32cc",
    "description": "car Trip Cancellation",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "travel",
      "item": [
        {
          "id": "cda34fbf-1ac0-4df4-a018-abeafe579ee9",
          "name": "car-trip-cancel",
          "request": {
            "url": "http://apim.expedia.com/x/m/api/cars/trip/cancel",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "emailAddress",
                  "value": "{}",
                  "disabled": false,
                  "description": "Email address of the traveler"
                },
                {
                  "key": "itineraryNumber",
                  "value": "{}",
                  "disabled": false,
                  "description": "Itinerary Number of the trip to cancel"
                }
              ]
            },
            "description": "car Trip Cancellation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bcf8817-9475-4168-b32f-e6d782ae170a"
            }
          ]
        }
      ]
    }
  ]
}