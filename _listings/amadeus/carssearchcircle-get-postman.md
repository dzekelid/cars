{
  "info": {
    "name": "Amadeus Get Cars Search",
    "_postman_id": "5557fb43-d089-4cec-b0b2-6b31a1f0bc95",
    "description": "With this API you can find out the price and type of car, for all car rental providers, in a specified geographical location.\n\nYou can quickly see the locations of car providers near a given point, and what cars are available to rent, and at what prices. This API is based on our car pricing service that gets live availability from car providers, and is used to power a variety of airline and travel agency websites.\n           \nResults are validated from car providers, and thus response times may take up to 10 seconds (response times are typically about 5s), and the number of concurrent calls is throttled per user to avoid flooding our provider's systems. However, this means the final result is guaranteed to be live and accurate.\n\nThe configuration of this API allows search for car rentals in the rental location where the car is picked up (at the start of the rental), is the same as the one where it will be dropped off.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "cars",
      "item": [
        {
          "id": "fa0c7bdb-b80a-4bfb-998b-936b5b128497",
          "name": "getCarsSearchCircle",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/cars/search-circle?currency=%7B%7D&drop_off=%7B%7D&lang=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&pick_up=%7B%7D&provider=%7B%7D&radius=%7B%7D&rate_class=%7B%7D&rate_filter=%7B%7D&rate_plan=%7B%7D&vehicle=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "With this API you can find out the price and type of car, for all car rental providers, in a specified geographical location"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2536b2d-d00d-4702-8e6f-714b0456cd19"
            }
          ]
        }
      ]
    }
  ]
}