{
  "info": {
    "name": "Amadeus",
    "_postman_id": "b0faf502-be80-45e4-a6c8-7ab46b3c8111",
    "description": "Amadeus API is a toolkit designed for travel agencies who want to develop their own travel products rather than using off-the-shelf solutions. With this tool, you can build your very own customised applications that link in a stable and secure dialogue with our Global Distribution System (GDS).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "airlines",
      "item": [
        {
          "id": "e9298467-139e-467a-9aaa-3a1bb134479d",
          "name": "getFlightsLowFareSearch",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/flights/low-fare-search?adults=%7B%7D&arrive_by=%7B%7D&children=%7B%7D&currency=%7B%7D&departure_date=%7B%7D&destination=%7B%7D&exclude_airlines=%7B%7D&include_airlines=%7B%7D&infants=%7B%7D&max_price=%7B%7D&nonstop=%7B%7D&number_of_results=%7B%7D&origin=%7B%7D&return_by=%7B%7D&return_date=%7B%7D&travel_class=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is the low fare search engine Amadeus uses to retrieve the best price for flights, based on our latest Master Pricer Travel Board technology"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1319de79-fc44-49a0-846e-23ed2986fa71"
            }
          ]
        }
      ]
    }
  ]
}