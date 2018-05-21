{
  "info": {
    "name": "Amadeus Get Travel Intelligence Top Destinations",
    "_postman_id": "ee6f83dc-7a06-4b8b-9705-f7a13284b309",
    "description": "The Top Flight Destinations API lets you find the most popular flight destinations from an origin during a period. This can help you answer questions like \"Where are most people from Paris going to during the month of September?\" The API is based on estimated flight traffic summary data from two journey points over a specific period. It returns up to 50 results, ordered by popularity, showing number of travelers as well as number of flights.\n\nThis estimated search is based on Amadeus' Travel Intelligence Engine, a high performance scalable cloud-based platform, born in the age of Big Data and purposely built for the industry bringing total flexibility and speed to business intelligence for travel. Please see amadeus.com/travelintelligence for more information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "travel",
      "item": [
        {
          "id": "d3c36de6-2f2d-491b-826d-e163f0910175",
          "name": "getTravelIntelligenceTopDestinations",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/travel-intelligence/top-destinations?number_of_results=%7B%7D&origin=%7B%7D&period=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Top Flight Destinations API lets you find the most popular flight destinations from an origin during a period"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "631d9981-47ea-43fb-9f20-f664b7375d48"
            }
          ]
        }
      ]
    }
  ]
}