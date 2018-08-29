{
  "info": {
    "name": "Amadeus",
    "_postman_id": "732d164c-97d8-4cac-bade-1f0000acc547",
    "description": "Amadeus API is a toolkit designed for travel agencies who want to develop their own travel products rather than using off-the-shelf solutions. With this tool, you can build your very own customised applications that link in a stable and secure dialogue with our Global Distribution System (GDS).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "airlines",
      "item": [
        {
          "id": "797ac80f-01c3-4a89-ac2e-39e7a6b8e098",
          "name": "getTravelIntelligenceFlightTraffic",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/travel-intelligence/flight-traffic?destination=%7B%7D&number_of_results_per_period=%7B%7D&origin=%7B%7D&period=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Flight Traffic API lets you find the origin and destination traffic summary between two journey points over a specified period"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe027bd3-31fd-43df-8f66-3a7c419f4a60"
            }
          ]
        }
      ]
    }
  ]
}