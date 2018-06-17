---
swagger: "2.0"
x-collection-name: Amadeus
x-complete: 0
info:
  title: Amadeus Get Flights Extensive Search
  description: |-
    The Extensive Flight Search allows you to find the prices of one-way or return flights between two airports over a large number of dates, and for a large variety of stay durations. The search doesn't return exact itineraries, but rather tells you the best price for a flight on a given day, for a stay of a given duration.

    The search is based on our Extreme Search platform, which continually caches a large number of flight search results from a list of origin cities to a variety of destinations. Since it's a cached search, the response time is fast, but not all origin airports are available. Here is a list of the currently supported origin-destination IATA location pairs. We try to keep this list as fresh as possible for you, but be aware that it may not always be exactly up-to-date and it can change without warning.

    That said, a price graph like this provides a powerful bargin shopping tool - allowing travelers with flexible itineraries to identify days on which they can get the cheapest flights to their destinations.
  contact:
    name: Amadeus Innovation and Research
    url: https://sandbox.amadeus.com
  version: 1.0.0
host: api.sandbox.amadeus.com
basePath: /v1.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /airports/autocomplete:
    get:
      summary: Get Airports Autocomplete
      description: "Using the term parameter and given the start of any word in an
        airport's official name, a city name, or the start of an IATA code, this API
        provides the full name and IATA location code of the city or airport, for
        use in flight searches. Only major cities and civilian airports with several
        commercial flights per week are included by default. The response provides
        up to 20 possible matches, sorted by importance, in a JQuery UI Autocomplete
        compatible format. This sample implementation using JQuery UI may help. This
        API uses data from the OpenTravelData project.\n \nBy only using the country
        parameter, this API is also able to find all the IATA location codes associated
        with a country. Both term and country parameters can be used together to filter
        the results accordingly.          \n\nThe value returned is the IATA location
        code. The label returned is always in UTF-8 format, with the airport official
        name (which is often in the native language), in the format of English City
        Name (if not already included in the airport name)."
      operationId: getAirportsAutocomplete
      x-api-path-slug: airportsautocomplete-get
      parameters:
      - in: query
        name: all_airports
        description: Boolean to include or not all airports, no matter their traffic
          rank
      - in: query
        name: country
        description: Identified a country based of a ISO 3166-1 alpha-2 code
      - in: query
        name: term
        description: Search keyword that should represent the start of a word in a
          city or airport name
      responses:
        200:
          description: OK
      tags:
      - Airlines
      - Airports
      - Autocomplete
  /airports/nearest-relevant:
    get:
      summary: Get Airports Nearest Relevant
      description: |-
        This service gives the most relevant airports in a radius of 500 km around the given coordinates. The relevance of an airport is computed by dividing the number of airport movements (take offs and landings) by the distance from the point. This causes the relevance of an airport to increase exponentially as you approach it.

        To minimize response time, all distances are computed as a great-circle distance from the provided coordinates to the airport coordinates, and thus do not take into account traffic conditions, international boundaries, mountains, water, or other elements that might make the a nearby airport hard to reach.

        Only civilian airports with at least several commercial flights per week are included in the results.

        The result is a list of airports sorted by decreasing relevance. It always contains the nearest airport with significant commercial traffic. You can freely download the point of reference information used by this API from the Open Travel Data project.
      operationId: getAirportsNearestRelevant
      x-api-path-slug: airportsnearestrelevant-get
      parameters:
      - in: query
        name: latitude
        description: Latitude location to be at the center of your search circle
      - in: query
        name: longitude
        description: Longitude location to be at the center of your search circle
      responses:
        200:
          description: OK
      tags:
      - Airlines
      - Airports
      - Nearest
      - Relevant
  /cars/search-airport:
    get:
      summary: Get Cars Search Airport
      description: "With this API you can find out the price and type of car, for
        all car rental providers, near a specified airport.\n\nYou can quickly see
        the locations of car providers near a given airport, and what cars are available
        to rent, and at what prices. This API is based on our car pricing service
        that gets live availability from car providers, and is used to power a variety
        of airline and travel agency websites.\n           \nResults are validated
        from car providers, and thus response times may take up to 10 seconds (response
        times are typically about 5s), and the number of concurrent calls is throttled
        per user to avoid flooding our provider's systems. However, this means the
        final result is guaranteed to be live and accurate.\n\nThe configuration of
        this API allows search for car rentals in the rental location where the car
        is picked up (at the start of the rental), is the same as the one where it
        will be dropped off."
      operationId: getCarsSearchAirport
      x-api-path-slug: carssearchairport-get
      parameters:
      - in: query
        name: currency
        description: The preferred currency to use when displaying prices and rates
          related to the car rental
      - in: query
        name: drop_off
        description: Date at which the car rental will end and the car will be returned
          to the rental location
      - in: query
        name: lang
        description: The preferred language of the content related to each car rental
      - in: query
        name: location
        description: The IATA code of the airport at which the car will be rented
      - in: query
        name: pick_up
        description: Date on which the car rental will be collected from the car rental
          location
      - in: query
        name: provider
        description: 2 character car rental provider code
      - in: query
        name: rate_class
        description: Allows to request specific rate types
      - in: query
        name: rate_filter
        description: Defines the types of rates to be returned in the output
      - in: query
        name: rate_plan
        description: Qualifies the rate depending on the pickup date and the rental
          duration
      - in: query
        name: vehicle
        description: Specifies the type of vehicle to be rented
      responses:
        200:
          description: OK
      tags:
      - Cars
      - Search
      - Airport
  /cars/search-circle:
    get:
      summary: Get Cars Search
      description: "With this API you can find out the price and type of car, for
        all car rental providers, in a specified geographical location.\n\nYou can
        quickly see the locations of car providers near a given point, and what cars
        are available to rent, and at what prices. This API is based on our car pricing
        service that gets live availability from car providers, and is used to power
        a variety of airline and travel agency websites.\n           \nResults are
        validated from car providers, and thus response times may take up to 10 seconds
        (response times are typically about 5s), and the number of concurrent calls
        is throttled per user to avoid flooding our provider's systems. However, this
        means the final result is guaranteed to be live and accurate.\n\nThe configuration
        of this API allows search for car rentals in the rental location where the
        car is picked up (at the start of the rental), is the same as the one where
        it will be dropped off."
      operationId: getCarsSearchCircle
      x-api-path-slug: carssearchcircle-get
      parameters:
      - in: query
        name: currency
        description: The preferred currency to use when displaying prices and rates
          related to the car rental
      - in: query
        name: drop_off
        description: Date at which the car rental will end and the car will be returned
          to the rental location
      - in: query
        name: lang
        description: The preferred language of the content related to each car rental
      - in: query
        name: latitude
        description: Latitude of the center of the search
      - in: query
        name: longitude
        description: Longitude of the center of the search
      - in: query
        name: pick_up
        description: Date on which the car rental will be collected from the car rental
          location
      - in: query
        name: provider
        description: 2 character car rental provider code
      - in: query
        name: radius
        description: Radius around the center to look for hotels in kilometers (km)
      - in: query
        name: rate_class
        description: Allows to request specific rate types
      - in: query
        name: rate_filter
        description: Defines the types of rates to be returned in the output
      - in: query
        name: rate_plan
        description: Qualifies the rate depending on the pickup date and the rental
          duration
      - in: query
        name: vehicle
        description: Specifies the type of vehicle to be rented
      responses:
        200:
          description: OK
      tags:
      - Cars
      - Search
      - Circle
  /flights/affiliate-search:
    get:
      summary: Get Flights Affiliate Search
      description: "The Flight Affiliate Search API combines Amadeus' flight search
        technology with Travel Audience's Connect API partners to provide a unique
        flight search, where all results come with deep-links to book the flight at
        a partner's website. The API will let you easily provide the traveler with
        a path to book flights from your application.\nTravel Audience Connect partners
        include\n\n  CityJet, Air Europa and TAP in Western Europe,\n  Ural Airlines
        in Russia, \n  Avianca Brazil  and\n  JAL in East Asia\n\n\nOnly Travel Audience
        Connect partner airlines are searched. For an up-to-date list of routes, see
        the route maps on each partners respective websites above. You can earn commission
        using the deep links provided in the search results if you sign up for an
        account at connect.travelaudience.com."
      operationId: getFlightsAffiliateSearch
      x-api-path-slug: flightsaffiliatesearch-get
      parameters:
      - in: query
        name: adults
        description: The number of adult (age 12 and over) passengers traveling on
          this flight
      - in: query
        name: children
        description: The number of child (younger than age 12 on date of departure)
          passengers traveling on this flight who will each have their own separate
          seat
      - in: query
        name: currency
        description: The preferred currency for the results
      - in: query
        name: departure_date
        description: The date on which the traveler will depart from the origin to
          go to the destination
      - in: query
        name: destination
        description: IATA code of the city to which the traveler is going
      - in: query
        name: exclude_merchants
        description: If specified, no results will include any flights where any of
          these airlines is the marketing carrier
      - in: query
        name: include_merchants
        description: If specified, all results will include at least one flight where
          one or more of these airlines is the marketing carrier
      - in: query
        name: infants
        description: The number of infant (younger than age 2 on date of departure)
          passengers traveling on this flight
      - in: query
        name: max_price
        description: Maximum price of trips to find in the result set, in USD (US
          dollars) unless some other currency code is specified
      - in: query
        name: mobile
        description: Setting this to true will show mobile web deeplinks
      - in: query
        name: origin
        description: City code from which the traveler will depart
      - in: query
        name: return_date
        description: The date on which the traveler will depart from the destination
          to return to the origin
      responses:
        200:
          description: OK
      tags:
      - Airlines
      - Flights
      - Affiliate
      - Search
  /flights/extensive-search:
    get:
      summary: Get Flights Extensive Search
      description: |-
        The Extensive Flight Search allows you to find the prices of one-way or return flights between two airports over a large number of dates, and for a large variety of stay durations. The search doesn't return exact itineraries, but rather tells you the best price for a flight on a given day, for a stay of a given duration.

        The search is based on our Extreme Search platform, which continually caches a large number of flight search results from a list of origin cities to a variety of destinations. Since it's a cached search, the response time is fast, but not all origin airports are available. Here is a list of the currently supported origin-destination IATA location pairs. We try to keep this list as fresh as possible for you, but be aware that it may not always be exactly up-to-date and it can change without warning.

        That said, a price graph like this provides a powerful bargin shopping tool - allowing travelers with flexible itineraries to identify days on which they can get the cheapest flights to their destinations.
      operationId: getFlightsExtensiveSearch
      x-api-path-slug: flightsextensivesearch-get
      parameters:
      - in: query
        name: aggregation_mode
        description: Specifies the granularity of results to be found
      - in: query
        name: departure_date
        description: Range of dates between which the traveler could depart
      - in: query
        name: destination
        description: IATA code of the city to which the traveler is going
      - in: query
        name: direct
        description: Limit the search to results that do not require the passenger
          to change plane?
      - in: query
        name: duration
        description: The allowed duration or range of durations of the trip, in days
      - in: query
        name: max_price
        description: Maximum price of trips to find in the result set, in the currency
          specified for this origin and destination pair in the cache contents spreadsheet
      - in: query
        name: one-way
        description: When set to true, the query will be for a single trip from the
          origin to the destination
      - in: query
        name: origin
        description: IATA code of the city from which the traveler will depart
      responses:
        200:
          description: OK
      tags:
      - Airlines
      - Flights
      - Extensive
      - Search
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