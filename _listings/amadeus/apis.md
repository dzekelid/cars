---
name: Amadeus
x-slug: amadeus
description: Amadeus travel technology helps businesses connect to the global travel
  ecosystem, manage operations more effectively and serve travellers better than ever
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
x-kinRank: "8"
x-alexaRank: "4309"
tags: Cars
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/cars/master/_listings/amadeus/apis.md
specificationVersion: "0.14"
apis:
- name: Amadeus - Get Cars Search Airport
  x-api-slug: carssearchairport-get
  description: "With this API you can find out the price and type of car, for all
    car rental providers, near a specified airport.\n\nYou can quickly see the locations
    of car providers near a given airport, and what cars are available to rent, and
    at what prices. This API is based on our car pricing service that gets live availability
    from car providers, and is used to power a variety of airline and travel agency
    websites.\n           \nResults are validated from car providers, and thus response
    times may take up to 10 seconds (response times are typically about 5s), and the
    number of concurrent calls is throttled per user to avoid flooding our provider's
    systems. However, this means the final result is guaranteed to be live and accurate.\n\nThe
    configuration of this API allows search for car rentals in the rental location
    where the car is picked up (at the start of the rental), is the same as the one
    where it will be dropped off."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cars/master/_listings/amadeus/carssearchairport-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cars/master/_listings/amadeus/carssearchairport-get-openapi.md
- name: Amadeus - Get Cars Search
  x-api-slug: carssearchcircle-get
  description: "With this API you can find out the price and type of car, for all
    car rental providers, in a specified geographical location.\n\nYou can quickly
    see the locations of car providers near a given point, and what cars are available
    to rent, and at what prices. This API is based on our car pricing service that
    gets live availability from car providers, and is used to power a variety of airline
    and travel agency websites.\n           \nResults are validated from car providers,
    and thus response times may take up to 10 seconds (response times are typically
    about 5s), and the number of concurrent calls is throttled per user to avoid flooding
    our provider's systems. However, this means the final result is guaranteed to
    be live and accurate.\n\nThe configuration of this API allows search for car rentals
    in the rental location where the car is picked up (at the start of the rental),
    is the same as the one where it will be dropped off."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Marketplace, Technology, Travel, Transportation, Airlines, API Provider, Hotels,
    Profiles, Relative Data, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cars/master/_listings/amadeus/carssearchcircle-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cars/master/_listings/amadeus/carssearchcircle-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://amadeus.api.gallery.streamdata.io
- type: x-api-stack
  url: http://amadeus.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/amadeus
- type: x-documentation
  url: https://sandbox.amadeus.com/api-catalog
- type: x-github
  url: https://github.com/AmadeusITGroup
- type: x-privacy-policy
  url: http://www.amadeus.com/web/amadeus/en_1A-corporate/Amadeus-Home/Amadeus_IT_Group_SA-Legal-notices-2014/1319560218660-Page-AMAD_Detail_PopUp_Ppal?assetid=1319607040997&assettype=DataProtection_C
- type: x-sandbox
  url: https://sandbox.amadeus.com
- type: x-twitter
  url: https://twitter.com/amadeusinnov
- type: x-website
  url: https://amadeus.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---