{
  "info": {
    "name": "Amadeus",
    "_postman_id": "a4594cae-9f13-46d7-9d06-380ee87e035f",
    "description": "Amadeus API is a toolkit designed for travel agencies who want to develop their own travel products rather than using off-the-shelf solutions. With this tool, you can build your very own customised applications that link in a stable and secure dialogue with our Global Distribution System (GDS).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "airlines",
      "item": [
        {
          "id": "6898d559-f48d-48bb-80bd-4927237ec249",
          "name": "getFlightsInspirationSearch",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/flights/inspiration-search?aggregation_mode=%7B%7D&departure_date=%7B%7D&destination=%7B%7D&direct=%7B%7D&duration=%7B%7D&max_price=%7B%7D&one-way=%7B%7D&origin=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Inspiration Flight Search allows you to find the prices of one-way and return flights from an origin city without necessarily having a destination, or even a flight date, in mind"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3bf5553-7d51-4118-a7ea-cddc46876199"
            }
          ]
        }
      ]
    }
  ]
}