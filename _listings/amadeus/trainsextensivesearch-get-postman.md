{
  "info": {
    "name": "Amadeus Get Trains Extensive Search",
    "_postman_id": "94a1f495-5574-414e-8442-bfef4751de20",
    "description": "This API allows you to search trains availability and prices for a single day or date range. It's based on our Rail Instant Search technology, providing you with immediate results from our rail search cache.\n\nThis API has content from SNCF (French trains).\n            \nThe content is also restricted to single-leg trips - where a single train takes you directly from the origin to the destination.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "trains",
      "item": [
        {
          "id": "9f374674-cd06-463c-b494-d67ba3d36a1e",
          "name": "getTrainsExtensiveSearch",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/trains/extensive-search?departure_date=%7B%7D&destination=%7B%7D&origin=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API allows you to search trains availability and prices for a single day or date range"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f755222-cd99-45fe-9d54-e45bd668c739"
            }
          ]
        }
      ]
    }
  ]
}