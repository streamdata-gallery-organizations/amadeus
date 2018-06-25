---
name: Amadeus
x-slug: amadeus
description: Amadeus travel technology helps businesses connect to the global travel
  ecosystem, manage operations more effectively and serve travellers better than ever
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
x-kinRank: "8"
x-alexaRank: "4309"
tags: Amadeus
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/apis.md
specificationVersion: "0.14"
apis:
- name: Amadeus Get Airports Autocomplete
  x-api-slug: amadeus
  description: "Using the term parameter and given the start of any word in an airport's
    official name, a city name, or the start of an IATA code, this API provides the
    full name and IATA location code of the city or airport, for use in flight searches.
    Only major cities and civilian airports with several commercial flights per week
    are included by default. The response provides up to 20 possible matches, sorted
    by importance, in a JQuery UI Autocomplete compatible format. This sample implementation
    using JQuery UI may help. This API uses data from the OpenTravelData project.\n
    \nBy only using the country parameter, this API is also able to find all the IATA
    location codes associated with a country. Both term and country parameters can
    be used together to filter the results accordingly.          \n\nThe value returned
    is the IATA location code. The label returned is always in UTF-8 format, with
    the airport official name (which is often in the native language), in the format
    of English City Name (if not already included in the airport name)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//airports/autocomplete
  tags: Airlines, Airports, Autocomplete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/airportsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/airportsautocomplete-get-openapi.md
- name: Amadeus Get Airports Nearest Relevant
  x-api-slug: amadeus
  description: |-
    This service gives the most relevant airports in a radius of 500 km around the given coordinates. The relevance of an airport is computed by dividing the number of airport movements (take offs and landings) by the distance from the point. This causes the relevance of an airport to increase exponentially as you approach it.

    To minimize response time, all distances are computed as a great-circle distance from the provided coordinates to the airport coordinates, and thus do not take into account traffic conditions, international boundaries, mountains, water, or other elements that might make the a nearby airport hard to reach.

    Only civilian airports with at least several commercial flights per week are included in the results.

    The result is a list of airports sorted by decreasing relevance. It always contains the nearest airport with significant commercial traffic. You can freely download the point of reference information used by this API from the Open Travel Data project.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//airports/nearest-relevant
  tags: Airlines, Airports, Nearest, Relevant
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/airportsnearestrelevant-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/airportsnearestrelevant-get-openapi.md
- name: Amadeus Get Cars Search Airport
  x-api-slug: amadeus
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
  baseURL: https://api.sandbox.amadeus.com//v1.2//cars/search-airport
  tags: Cars, Search, Airport
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/carssearchairport-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/carssearchairport-get-openapi.md
- name: Amadeus Get Cars Search
  x-api-slug: amadeus
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
  baseURL: https://api.sandbox.amadeus.com//v1.2//cars/search-circle
  tags: Cars, Search, Circle
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/carssearchcircle-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/carssearchcircle-get-openapi.md
- name: Amadeus Get Flights Affiliate Search
  x-api-slug: amadeus
  description: "The Flight Affiliate Search API combines Amadeus' flight search technology
    with Travel Audience's Connect API partners to provide a unique flight search,
    where all results come with deep-links to book the flight at a partner's website.
    The API will let you easily provide the traveler with a path to book flights from
    your application.\nTravel Audience Connect partners include\n\n  CityJet, Air
    Europa and TAP in Western Europe,\n  Ural Airlines in Russia, \n  Avianca Brazil
    \ and\n  JAL in East Asia\n\n\nOnly Travel Audience Connect partner airlines are
    searched. For an up-to-date list of routes, see the route maps on each partners
    respective websites above. You can earn commission using the deep links provided
    in the search results if you sign up for an account at connect.travelaudience.com."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//flights/affiliate-search
  tags: Airlines, Flights, Affiliate, Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/flightsaffiliatesearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/flightsaffiliatesearch-get-openapi.md
- name: Amadeus Get Flights Extensive Search
  x-api-slug: amadeus
  description: |-
    The Extensive Flight Search allows you to find the prices of one-way or return flights between two airports over a large number of dates, and for a large variety of stay durations. The search doesn't return exact itineraries, but rather tells you the best price for a flight on a given day, for a stay of a given duration.

    The search is based on our Extreme Search platform, which continually caches a large number of flight search results from a list of origin cities to a variety of destinations. Since it's a cached search, the response time is fast, but not all origin airports are available. Here is a list of the currently supported origin-destination IATA location pairs. We try to keep this list as fresh as possible for you, but be aware that it may not always be exactly up-to-date and it can change without warning.

    That said, a price graph like this provides a powerful bargin shopping tool - allowing travelers with flexible itineraries to identify days on which they can get the cheapest flights to their destinations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//flights/extensive-search
  tags: Airlines, Flights, Extensive, Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/flightsextensivesearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/flightsextensivesearch-get-openapi.md
- name: Amadeus Get Flights Inspiration Search
  x-api-slug: amadeus
  description: |-
    The Inspiration Flight Search allows you to find the prices of one-way and return flights from an origin city without necessarily having a destination, or even a flight date, in mind. The search doesn't return a distinct set of price options, but rather, can tell you the price of flying from a given city to some destination, for a trip of a given duration, that falls within a given date range.

    The search is based on our Extreme Search platform, which continually caches a large number of flight search results from a list of origin cities to a variety of destinations. Since it's a cached search, the response time is fast, but not all origin airports are available. Here is a list of the currently supported origin-destination IATA location pairs. We try to keep this list as fresh as possible for you, but be aware that it may not always be exactly up-to-date and it can change without warning.

    Despite this limitation don't underestimate the power of this API. Thanks to its quick response speed you can easily pair it with other APIs to provide a low fare and inspiration for any destination. For example, you can could combine it with a event search API and suggest a total price to see go and see an concert or a game in a selection of cities.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//flights/inspiration-search
  tags: Airlines, Flights, Inspiration, Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/flightsinspirationsearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/flightsinspirationsearch-get-openapi.md
- name: Amadeus Get Flights Low Fare Search
  x-api-slug: amadeus
  description: "This is the low fare search engine Amadeus uses to retrieve the best
    price for flights, based on our latest Master Pricer Travel Board technology.
    This document describes how to make a low fare search and how to handle the returned
    messages.\n\nThe message is composed of multiple results for given request. A
    result is defined by a unique combination of price, tax, passenger type, fare
    type, cabin, and availability for each requested segment. \n\nA result is then
    composed of single or multiple itineraries. Each itinerary is composed of an outbound
    leg, and, if a return date was specified, an inbound leg. Each leg is composed
    of a list of one or more flights, that the traveller will be required to take
    in order to get from the origin airport to the destination airport."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//flights/low-fare-search
  tags: Airlines, Flights, Low, Fare, Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/flightslowfaresearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/flightslowfaresearch-get-openapi.md
- name: Amadeus Get Hotels Search Airport
  x-api-slug: amadeus
  description: |-
    A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices. With this API you can find out the price of the cheapest daily rate for all hotels near a given airport.

    This API allows you to quickly see the locations of hotels near a given airport, and what prices in that area look like. Note that hotel images are not available to users outside of Amadeus, as we are not licensed to redistribute them. The API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//hotels/search-airport
  tags: Hotels, Search, Airport
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/hotelssearchairport-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/hotelssearchairport-get-openapi.md
- name: Amadeus Get Hotels Search Box
  x-api-slug: amadeus
  description: "A fast Hotel shopping API to see which hotels are available in a given
    area, on a given day and displays their lowest prices. With this API you can find
    out the price of the cheapest daily rate for all hotels within a specified geographical
    region.\n\nThis API allows you to quickly see the hotel locations in a region,
    and what prices in that area look like,  as well as the check-in and check-out
    dates, and get a list of up to 140 properties (names, codes, image, amenities)
    with their locations and rates. Optional parameters such as currency and maximum
    rates, amenities or hotel chain codes are also available and can be used to narrow
    down the results. More optional parameters such as show_sold_out & rooms can be
    used to show sold out rooms and all available rooms.\n            \nThe API is
    based on our high-speed hotel pricing cache, which is also used to power the Amadeus
    Hotel Search Engine application. Results are returned very quickly, response times
    are generally under 2s. Our cache has great global coverage and is constantly
    refreshed with the latest prices."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//hotels/search-box
  tags: Hotels, Search, Box
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/hotelssearchbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/hotelssearchbox-get-openapi.md
- name: Amadeus Get Hotels Search Circle
  x-api-slug: amadeus
  description: "A fast Hotel shopping API to see which hotels are available in a given
    area, on a given day and displays their lowest prices. With this API you can find
    out the price of the cheapest daily rate for all hotels within a specified radius
    of a point.\n\nThis API allows you to quickly see the hotel locations in a region,
    and what prices in that area look like,  as well as the check-in and check-out
    dates, and get list of up to 140 properties (names, codes, image, amenities) with
    their locations and rates. Optional parameters such as currency and maximum rates,
    amenities or hotel chain codes are also available and can be used to narrow down
    the results. More optional parameters such as show_sold_out & rooms can be used
    to show sold out rooms and all available rooms. \n\nThe API is based on our high-speed
    hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine
    application. Results are returned very quickly, response times are generally under
    2s. Our cache has great global coverage and is constantly refreshed with the latest
    prices."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//hotels/search-circle
  tags: Hotels, Search, Circle
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/hotelssearchcircle-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/hotelssearchcircle-get-openapi.md
- name: Amadeus Get Hotels Property Code
  x-api-slug: amadeus
  description: "This API allows you to quickly see the detailed information of a single
    hotel, including descriptions, address, GPS location, amenities, awards, lowest
    priced room and all room prices and booking information. \n\nThis API gives you
    more information on a specific property. Optional parameters such as show_sold_out
    & rooms can be used to show sold out rooms and all available rooms. \n\nThe API
    is based on our high-speed hotel pricing cache, which is also used to power the
    Amadeus Hotel Search Engine application. Results are returned very quickly, response
    times are generally under 2s. Our cache has great global coverage and is constantly
    refreshed with the latest prices."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//hotels/{property_code}
  tags: Hotels, Property, Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/hotelsproperty-code-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/hotelsproperty-code-get-openapi.md
- name: Amadeus Get Location Code
  x-api-slug: amadeus
  description: |-
    This service retrieves the location information corresponding to a IATA city or airport code.

    When provided with an IATA code, the service determines whether this code could relate to a city code, an airport code or both. If the city could contain multiple airports, it will return all possible airports that correspond to that city code.

    This API is based on the Amadeus supported Geobases open-source project. If you wish to make your own database with all IATA location information, in order to get faster reponses, you can download the latest raw data from their github page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//location/{code}
  tags: Location, Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/locationcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/locationcode-get-openapi.md
- name: Amadeus Get Points Of Interest Yapq Search Circle
  x-api-slug: amadeus
  description: "Amadeus has partnered with YapQ to bring you point of interest APIs
    with the goal of offering you unbiased ratings of landmarks and tourist attractions.
    YapQ rates places according to their interest on social media and provides Wikipedia
    content and Geonames ID at a given location. \nYapQ's service indexes millions
    of points around the world, and provides content in 12 different languages. This
    allows you to ensure you catch the must-see sights at a specific YapQ supported
    location.\nEach point of interest comes with links to content, grading information,
    location and directions to help make discovering your destination easy and fun.\nThis
    service is still under active development, and the response format may change
    without warning. We'd be interested in your feedback - send us an email."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//points-of-interest/yapq-search-circle
  tags: Points, Of, Interest, Yapq, Search, Circle
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/pointsofinterestyapqsearchcircle-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/pointsofinterestyapqsearchcircle-get-openapi.md
- name: Amadeus Get Points Of Interest Yapq Search Text
  x-api-slug: amadeus
  description: "Amadeus has partnered with YapQ to bring you point of interest APIs
    with the goal of offering you unbiased ratings of landmarks and tourist attractions.
    YapQ rates these points according to their interest on social media and provides
    Wikipedia content and Geonames ID in a given city. \nYapQ's service indexes millions
    of points around the world, and provides content in 12 different languages. This
    allows you to ensure you catch the must-see sights in a YapQ supported city.\nEach
    point of interest comes with links to content, grading information, location and
    directions to help make discovering your destination easy and fun.\nThis service
    is still under active development, and the response format may change without
    warning. We'd be interested in your feedback - send us an email."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//points-of-interest/yapq-search-text
  tags: Points, Of, Interest, Yapq, Search, Text
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/pointsofinterestyapqsearchtext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/pointsofinterestyapqsearchtext-get-openapi.md
- name: Amadeus Get Rail Station
  x-api-slug: amadeus
  description: Get rail station
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//rail-station/{id}
  tags: Rail, Station
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/railstationid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/railstationid-get-openapi.md
- name: Amadeus Get Rail Stations Autocomplete
  x-api-slug: amadeus
  description: |-
    Given the start of any word in a rail station's official name, as a term, this API provides the full name and rail station ID of a rail station for use in searches. The response provides an array of up to 20 possible matches, sorted by passenger traffic, in a JQuery Autocomplete compatible format.

    The value returned is the UIC station code. The label returned is always in UTF-8 format, with the station's official name (which is often in the native language). Agglomeration station codes may also be returned.

    Note that only French and Italian rail stations are supported by the Rail Station Autocomplete API
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//rail-stations/autocomplete
  tags: Rail, Stations, Autocomplete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/railstationsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/railstationsautocomplete-get-openapi.md
- name: Amadeus Get Trains Extensive Search
  x-api-slug: amadeus
  description: "This API allows you to search trains availability and prices for a
    single day or date range. It's based on our Rail Instant Search technology, providing
    you with immediate results from our rail search cache.\n\nThis API has content
    from SNCF (French trains).\n            \nThe content is also restricted to single-leg
    trips - where a single train takes you directly from the origin to the destination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//trains/extensive-search
  tags: Trains, Extensive, Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/trainsextensivesearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/trainsextensivesearch-get-openapi.md
- name: Amadeus Get Trains Schedule Search
  x-api-slug: amadeus
  description: |-
    This API allows you to find all the possible destinations in the Rail Instant Search cache (used by Extensive Search above) from a given origin station on a given day. You can use this to help build network maps, journey planners or provide inspiration for rail travel.

    This API has continuous content from SNCF.
    All the options returned are single-leg trips - where a single train takes you directly from the origin to the destination. In general, only departure dates up to 90 days in the future are supported

    Currently agglomeration stations are not supported
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//trains/schedule-search
  tags: Trains, Schedule, Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/trainsschedulesearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/trainsschedulesearch-get-openapi.md
- name: Amadeus Get Travel Intelligence Flight Traffic
  x-api-slug: amadeus
  description: "The Flight Traffic API lets you find the origin and destination traffic
    summary between two journey points over a specified period.\nThe search returns
    number of flights & travelers for each origin and destination, ordered by popularity,
    for each month specified within the search period. This search can help you answer
    questions like \"Where are people from Los Angeles traveling to between January
    and April of 2015?\" or \"Which is the most popular month for New Yorkers to travel
    last year?\". \nThis search is based on Amadeus' Travel Intelligence Engine, a
    high performance scalable cloud-based platform, born in the age of Big Data and
    purposely built for the industry bringing total flexibility and speed to business
    intelligence for travel. Please see amadeus.com/travelintelligence for more information."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//travel-intelligence/flight-traffic
  tags: Airlines, Travel, Intelligence, Flight, Traffic
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/travelintelligenceflighttraffic-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/travelintelligenceflighttraffic-get-openapi.md
- name: Amadeus Get Travel Intelligence Top Destinations
  x-api-slug: amadeus
  description: |-
    The Top Flight Destinations API lets you find the most popular flight destinations from an origin during a period. This can help you answer questions like "Where are most people from Paris going to during the month of September?" The API is based on estimated flight traffic summary data from two journey points over a specific period. It returns up to 50 results, ordered by popularity, showing number of travelers as well as number of flights.

    This estimated search is based on Amadeus' Travel Intelligence Engine, a high performance scalable cloud-based platform, born in the age of Big Data and purposely built for the industry bringing total flexibility and speed to business intelligence for travel. Please see amadeus.com/travelintelligence for more information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//travel-intelligence/top-destinations
  tags: Travel, Intelligence, Top, Destinations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/travelintelligencetopdestinations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/travelintelligencetopdestinations-get-openapi.md
- name: Amadeus Get Travel Intelligence Top Searches
  x-api-slug: amadeus
  description: "The Top Flight Search allows you to find number of estimated searches
    from an origin, optionally a destination, within a time period when travelers
    are performing the searches. \nThe search is based on queries performed from within
    a country (also refers to as market) and returns up to 50 results, ordered by
    popularity, showing number of searches for most searched destination with its
    previous year comparison. This search also shows patterns on how travelers are
    searching for flights, revealing where, when and for how long they\u2019re planning
    to travel. See\nTrip Durations(How long are the trips planned for?) and\n Advance
    Search Period (How long before departures do travelers start searching for their
    trips?)\n\nThis estimated search is based on Amadeus' Travel Intelligence Engine,
    a high performance scalable cloud-based platform, born in the age of Big Data
    and purposely built for the industry bringing total flexibility and speed to business
    intelligence for travel. Please see amadeus.com/travelintelligence for more information."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//travel-intelligence/top-searches
  tags: Travel, Intelligence, Top, Searches
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/travelintelligencetopsearches-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/travelintelligencetopsearches-get-openapi.md
- name: Amadeus Get Travel Record Record Locator
  x-api-slug: amadeus
  description: |-
    Note: This API requires the use of HTTPS

    This service retrieves a travel record (also sometimes referred to as a PNR) for a given journey when provided with Record Locator to identify a travel record, along with the last name of any traveler who is marked as a passenger on this record.

    The API provides detailed information on a given record, including any air, car, hotel or rail reservations, as well as passenger details, and contact frequent traveler information for each passenger when available. You can use this to provide a wide variety of pre-trip or in-trip services.

    Note that this API transmits sensitive personal data about a traveler's journey. We work hard to ensure that we comply with all the legal requirements this entails, and as an application owner, you need to do so too - we don't want you to get in trouble! This paragraph, or anything else in our documentation, does not constitute legal advice, it's just to give you an idea of some of the potential issues that you may encounter. Please check your legal obligations regarding the use of this data before implementing this API

    In most countries, the data in the returned travel record is considered to be the property of the traveler. In order to ensure that you are acting on behalf of the traveler, we require you to provide the traveler's last name in addition to the record locator when you make a call to this API. You should ensure that you have consent from the traveler before retrieving this record, in some countries this is a legal requirement - please respect this appropriately.

    Our data center is based in Europe, so there is a legal requirement that you to access this API over a secure connection. If you plan to store the information returned by this API, ensure you comply with storage requirements for European data, in addition to those of your local country. For example, there are strict requirements on the caching of retrieved travel records, so please ensure the cache control HTTP headers in the response are respected.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2//travel-record/{record_locator}
  tags: Travel, Record, Record, Locator
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/travelrecordrecord-locator-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/travelrecordrecord-locator-get-openapi.md
- name: Amadeus
  x-api-slug: amadeus
  description: Amadeus travel technology helps businesses connect to the global travel
    ecosystem, manage operations more effectively and serve travellers better than
    ever
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28139-sandbox-amadeus-com.jpg
  humanURL: https://amadeus.com
  baseURL: https://api.sandbox.amadeus.com//v1.2
  tags: Amadeus
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/amadeus/master/_listings/amadeus/openapi.md
x-common:
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