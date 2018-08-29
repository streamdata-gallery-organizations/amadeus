{
  "info": {
    "name": "Amadeus",
    "_postman_id": "afe6adcb-b8f6-4d62-88e6-a0ca63a095fa",
    "description": "Amadeus API is a toolkit designed for travel agencies who want to develop their own travel products rather than using off-the-shelf solutions. With this tool, you can build your very own customised applications that link in a stable and secure dialogue with our Global Distribution System (GDS).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "airlines",
      "item": [
        {
          "id": "4f915448-3382-415e-b733-93f0f0d69345",
          "name": "getAirportsAutocomplete",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/airports/autocomplete?all_airports=%7B%7D&country=%7B%7D&term=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Using the term parameter and given the start of any word in an airport's official name, a city name, or the start of an IATA code, this API provides the full name and IATA location code of the city or airport, for use in flight searches"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c05d0d7a-38eb-4873-88a6-1a7596fb9430"
            }
          ]
        }
      ]
    }
  ]
}