{
  "info": {
    "name": "Amadeus Get Travel Intelligence Top Searches",
    "_postman_id": "cc75ff93-0fb4-44c7-94c7-e9bf26e07a4e",
    "description": "The Top Flight Search allows you to find number of estimated searches from an origin, optionally a destination, within a time period when travelers are performing the searches. \nThe search is based on queries performed from within a country (also refers to as market) and returns up to 50 results, ordered by popularity, showing number of searches for most searched destination with its previous year comparison. This search also shows patterns on how travelers are searching for flights, revealing where, when and for how long they’re planning to travel. See\nTrip Durations(How long are the trips planned for?) and\n Advance Search Period (How long before departures do travelers start searching for their trips?)\n\nThis estimated search is based on Amadeus' Travel Intelligence Engine, a high performance scalable cloud-based platform, born in the age of Big Data and purposely built for the industry bringing total flexibility and speed to business intelligence for travel. Please see amadeus.com/travelintelligence for more information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "travel",
      "item": [
        {
          "id": "4cb60c43-26e7-4ea6-a50d-73e277399194",
          "name": "getTravelIntelligenceTopSearches",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/travel-intelligence/top-searches?country=%7B%7D&destination=%7B%7D&number_of_results=%7B%7D&origin=%7B%7D&period=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Top Flight Search allows you to find number of estimated searches from an origin, optionally a destination, within a time period when travelers are performing the searches"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa2312e6-0305-498a-9c95-594f9415237a"
            }
          ]
        }
      ]
    }
  ]
}