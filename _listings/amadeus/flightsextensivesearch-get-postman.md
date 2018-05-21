{
  "info": {
    "name": "Amadeus",
    "_postman_id": "e88a41af-fddb-44b6-8b0c-ef2facc5f35f",
    "description": "Amadeus API is a toolkit designed for travel agencies who want to develop their own travel products rather than using off-the-shelf solutions. With this tool, you can build your very own customised applications that link in a stable and secure dialogue with our Global Distribution System (GDS).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "airlines",
      "item": [
        {
          "id": "63b51451-b73f-46f5-a02e-ae94ba192d7b",
          "name": "getFlightsExtensiveSearch",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/flights/extensive-search?aggregation_mode=%7B%7D&departure_date=%7B%7D&destination=%7B%7D&direct=%7B%7D&duration=%7B%7D&max_price=%7B%7D&one-way=%7B%7D&origin=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Extensive Flight Search allows you to find the prices of one-way or return flights between two airports over a large number of dates, and for a large variety of stay durations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa165245-74bc-4ee5-a7b0-bda7c285973d"
            }
          ]
        }
      ]
    }
  ]
}