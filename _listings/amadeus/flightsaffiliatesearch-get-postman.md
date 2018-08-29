{
  "info": {
    "name": "Amadeus",
    "_postman_id": "aca7b07d-c351-427d-9724-684bbc5dbed1",
    "description": "Amadeus API is a toolkit designed for travel agencies who want to develop their own travel products rather than using off-the-shelf solutions. With this tool, you can build your very own customised applications that link in a stable and secure dialogue with our Global Distribution System (GDS).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "airlines",
      "item": [
        {
          "id": "4ce15adf-ccd7-4115-9ba0-d62d6ad67445",
          "name": "getFlightsAffiliateSearch",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/flights/affiliate-search?adults=%7B%7D&children=%7B%7D&currency=%7B%7D&departure_date=%7B%7D&destination=%7B%7D&exclude_merchants=%7B%7D&include_merchants=%7B%7D&infants=%7B%7D&max_price=%7B%7D&mobile=%7B%7D&origin=%7B%7D&return_date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Flight Affiliate Search API combines Amadeus' flight search technology with Travel Audience's Connect API partners to provide a unique flight search, where all results come with deep-links to book the flight at a partner's website"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec481a8d-e556-4a82-929a-86de3a51a62c"
            }
          ]
        }
      ]
    }
  ]
}