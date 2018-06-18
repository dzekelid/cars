---
swagger: "2.0"
x-collection-name: Expedia
x-complete: 1
info:
  title: Expedia
  description: expedia-mobile-api-documentation--brfont-colorblue-note-in-case-of-authorization-exception-just-a-hrefstaticmobileswaggeruiusersigninusersigninafont
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
  /m/api/cars/trip/checkout:
    post:
      summary: Checkout
      description: Mobile API Cars Checkout
      operationId: cars-checkout
      x-api-path-slug: mapicarstripcheckout-post
      parameters:
      - in: formData
        name: airlineCode
        description: Airline code of the travelers flight
      - in: formData
        name: city
        description: The city of the travelers billing address
      - in: formData
        name: country
        description: The 3 letter country code of the travelers billing address
      - in: formData
        name: creditCardNumber
        description: The credit card number used for this booking, if checking out
          with a new card
      - in: formData
        name: cvv
        description: The CVV of the travelers credit card used for this booking
      - in: formData
        name: doIThinkImSignedIn
        description: As a client I am checking-out with the assumption that I am signed
          in
      - in: formData
        name: expectedCardFee
        description: The expected credit card fee, as returned by the createTrip call
          in the validFormsOfPayment object for whatever credit card the user is paying
          with
      - in: formData
        name: expectedCardFeeCurrencyCode
        description: Three letter 4217 ISO currency code of the expected credit card
          fee
      - in: formData
        name: expectedFareCurrencyCode
        description: Three letter 4217 ISO currency code of the expected total price
      - in: formData
        name: expectedTotalFare
        description: The expected total price of the trip, matching exactly whatever
          the user last saw
      - in: formData
        name: expirationDateMonth
        description: The expiration date month of the credit card used for this booking
      - in: formData
        name: expirationDateYear
        description: The 4 digit expiration date year of the credit card used for
          this booking
      - in: formData
        name: flightNumber
        description: Flight number of the traveler
      - in: formData
        name: loyaltyNumber
        description: Loyalty number of the traveler
      - in: formData
        name: mainMobileTraveler.email
        description: This passengers email address
      - in: formData
        name: mainMobileTraveler.expediaEmailOptIn
        description: Whether to opt-in the users email to travel deals
      - in: formData
        name: mainMobileTraveler.firstName
        description: The first name of the traveler
      - in: formData
        name: mainMobileTraveler.lastName
        description: The last name of the traveler
      - in: formData
        name: mainMobileTraveler.middleName
        description: The middle name of the traveler
      - in: formData
        name: mainMobileTraveler.password
        description: The password provided by the expedia user
      - in: formData
        name: mainMobileTraveler.phone
        description: The phone number of the traveler
      - in: formData
        name: mainMobileTraveler.phoneCountryCode
        description: The country code of the phone number of the traveler
      - in: formData
        name: nameOnCard
        description: The card holders name
      - in: formData
        name: omniturePartnerId
        description: Omniture partner identification string
      - in: formData
        name: postalCode
        description: The postal code of the travelers billing address
      - in: formData
        name: prettyPrint
        description: If true, return JSON with tabs, spaces and newlines to be human
          readable
      - in: formData
        name: specialEquipments
        description: Special Equipments to be requested
      - in: formData
        name: state
        description: The state (or province) of the travelers billing address
      - in: formData
        name: storeCreditCardInUserProfile
        description: Indicates whether to save the credit card information as a stored
          credit card in the user profile
      - in: formData
        name: storedCreditCardId
        description: The GUID for the stored credit card information to be used for
          payment
      - in: formData
        name: streetAddress
        description: The street part of the credit card owners billing address
      - in: formData
        name: streetAddress2
        description: Apartment or suite number of the travelers billing address
      - in: formData
        name: suppressFinalBooking
        description: If true, do not actually charge for and book the trip, stop after
          creating the itinerary
      - in: formData
        name: tealeafTransactionId
        description: The unique transaction ID used in TeaLeaf PSR tracking
      - in: formData
        name: tripId
        description: The trip ID of an existing trip, from /api/flight/trip/create
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Cars
  /m/api/cars/trip/cancel:
    post:
      summary: Cancel Trip
      description: car Trip Cancellation
      operationId: car-trip-cancel
      x-api-path-slug: mapicarstripcancel-post
      parameters:
      - in: formData
        name: emailAddress
        description: Email address of the traveler
      - in: formData
        name: itineraryNumber
        description: Itinerary Number of the trip to cancel
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Cars
---