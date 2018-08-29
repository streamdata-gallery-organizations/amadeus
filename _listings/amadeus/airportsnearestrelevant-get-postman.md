{
  "info": {
    "name": "Amadeus",
    "_postman_id": "fb7e16a8-afee-4b7f-a5f6-c00ce68c53d7",
    "description": "Amadeus API is a toolkit designed for travel agencies who want to develop their own travel products rather than using off-the-shelf solutions. With this tool, you can build your very own customised applications that link in a stable and secure dialogue with our Global Distribution System (GDS).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "airlines",
      "item": [
        {
          "id": "5c260439-e672-4aeb-857f-0506cb2bc9ad",
          "name": "getAirportsNearestRelevant",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/airports/nearest-relevant?latitude=%7B%7D&longitude=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service gives the most relevant airports in a radius of 500 km around the given coordinates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd4e543e-4854-4f79-adec-4576a9a270c1"
            }
          ]
        }
      ]
    }
  ]
}