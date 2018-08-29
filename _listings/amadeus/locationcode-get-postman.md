{
  "info": {
    "name": "Amadeus Get Location Code",
    "_postman_id": "d3423742-7111-4423-99f8-02b6171ce221",
    "description": "This service retrieves the location information corresponding to a IATA city or airport code.\n\nWhen provided with an IATA code, the service determines whether this code could relate to a city code, an airport code or both. If the city could contain multiple airports, it will return all possible airports that correspond to that city code.\n\nThis API is based on the Amadeus supported Geobases open-source project. If you wish to make your own database with all IATA location information, in order to get faster reponses, you can download the latest raw data from their github page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "location",
      "item": [
        {
          "id": "6723183f-aa43-470e-9e6f-0ec1706062e2",
          "name": "getLocationCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sandbox.amadeus.com",
              "path": [
                "v1.2",
                "location/:code"
              ],
              "variable": [
                {
                  "id": "code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service retrieves the location information corresponding to a IATA city or airport code"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0e3a4c5-a407-4bc4-96ae-40916e51138b"
            }
          ]
        }
      ]
    }
  ]
}