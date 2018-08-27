{
  "info": {
    "name": "Expedia Create A Trip",
    "_postman_id": "11221689-c23d-4633-9ce5-bf67c0047117",
    "description": "Mobile API Cars Create Trip",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "travel",
      "item": [
        {
          "id": "21bd6d60-84ec-4af5-b702-24dabdda1d90",
          "name": "cars-create-trip",
          "request": {
            "url": "http://apim.expedia.com/x/m/api/cars/trip/create",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "expectedTotalFare",
                  "value": "{}",
                  "disabled": false,
                  "description": "The expected total price of the trip, matching exactly whatever the user last saw"
                },
                {
                  "key": "productKey",
                  "value": "{}",
                  "disabled": false,
                  "description": "The product ID (piid) you would like to create a trip"
                },
                {
                  "key": "tripName",
                  "value": "{}",
                  "disabled": false,
                  "description": "Name of this trip"
                }
              ]
            },
            "description": "Mobile API Cars Create Trip"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f4d1246-06bf-4319-bc0c-930d5a2a82c0"
            }
          ]
        }
      ]
    }
  ]
}