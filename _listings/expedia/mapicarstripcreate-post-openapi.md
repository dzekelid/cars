---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 0
info:
  title: Expedia Create A Trip
  description: Mobile API Cars Create Trip
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /m/api/cars/search/airport:
    get:
      summary: Search
      description: Mobile API Cars
      operationId: cars-search
      x-api-path-slug: mapicarssearchairport-get
      parameters:
      - in: query
        name: airportCode
        description: 3 letter airport code where you will be picking up and dropping
          off your rental car
      - in: query
        name: dropOffTime
        description: When you will pick up the car
      - in: query
        name: pickupTime
        description: When you will pick up the car
      - in: query
        name: vendorCode
        description: The vendor code to filter/limit search results
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Cars
  /m/api/cars/search/location:
    get:
      summary: Search
      description: Mobile API Cars
      operationId: cars-search
      x-api-path-slug: mapicarssearchlocation-get
      parameters:
      - in: query
        name: dropOffTime
        description: When you will pick up the car
      - in: query
        name: pickupLocation.lat
        description: The location (latitude) to search near
      - in: query
        name: pickupLocation.lon
        description: The location (longitude) to search near
      - in: query
        name: pickupTime
        description: When you will pick up the car
      - in: query
        name: searchRadius
        description: The max distance around the location to search in
      - in: query
        name: vendorCode
        description: The vendor code to filter/limit search results
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Cars
  /m/api/cars/search:
    get:
      summary: Search
      description: Mobile API Cars
      operationId: cars-search
      x-api-path-slug: mapicarssearch-get
      parameters:
      - in: query
        name: destinationAirportCode
        description: 3 letter airport code where you will dropping off your rental
          car
      - in: query
        name: dropOffLocation.lat
        description: The location (latitude) for drop off
      - in: query
        name: dropOffLocation.lon
        description: The location (longitude) for drop off
      - in: query
        name: dropOffTime
        description: When you will pick up the car
      - in: query
        name: originAirportCode
        description: 3 letter airport code where you will be picking up your rental
          car
      - in: query
        name: pickupLocation.lat
        description: The location (latitude) to search near
      - in: query
        name: pickupLocation.lon
        description: The location (longitude) to search near
      - in: query
        name: pickupTime
        description: When you will pick up the car
      - in: query
        name: searchRadius
        description: The max distance around the location to search in
      - in: query
        name: vendorCode
        description: The vendor code to filter/limit search results
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Cars
  /m/api/cars/trip/create:
    post:
      summary: Create A Trip
      description: Mobile API Cars Create Trip
      operationId: cars-create-trip
      x-api-path-slug: mapicarstripcreate-post
      parameters:
      - in: formData
        name: expectedTotalFare
        description: The expected total price of the trip, matching exactly whatever
          the user last saw
      - in: formData
        name: productKey
        description: The product ID (piid) you would like to create a trip
      - in: formData
        name: tripName
        description: Name of this trip
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Cars
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---