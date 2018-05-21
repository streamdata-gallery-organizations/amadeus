{
  "info": {
    "name": "Amadeus Get Hotels Search Airport",
    "_postman_id": "0d96255d-1b1a-4b02-ac94-21d00bb625e6",
    "description": "A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices. With this API you can find out the price of the cheapest daily rate for all hotels near a given airport.\n\nThis API allows you to quickly see the locations of hotels near a given airport, and what prices in that area look like. Note that hotel images are not available to users outside of Amadeus, as we are not licensed to redistribute them. The API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "hotels",
      "item": [
        {
          "id": "00dc1e86-cb2a-4ba8-9333-4f2a180f8b07",
          "name": "getHotelsSearchAirport",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/hotels/search-airport?all_rooms=%7B%7D&amenity=%7B%7D&chain=%7B%7D&check_in=%7B%7D&check_out=%7B%7D&currency=%7B%7D&lang=%7B%7D&location=%7B%7D&max_rate=%7B%7D&number_of_results=%7B%7D&radius=%7B%7D&show_sold_out=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75269c49-2dd4-4f43-8453-1831f42a162c"
            }
          ]
        }
      ]
    }
  ]
}