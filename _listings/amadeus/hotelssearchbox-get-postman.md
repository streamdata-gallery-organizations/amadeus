{
  "info": {
    "name": "Amadeus Get Hotels Search Box",
    "_postman_id": "b4f37045-64e6-47cc-b514-873dcf53f686",
    "description": "A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices. With this API you can find out the price of the cheapest daily rate for all hotels within a specified geographical region.\n\nThis API allows you to quickly see the hotel locations in a region, and what prices in that area look like,  as well as the check-in and check-out dates, and get a list of up to 140 properties (names, codes, image, amenities) with their locations and rates. Optional parameters such as currency and maximum rates, amenities or hotel chain codes are also available and can be used to narrow down the results. More optional parameters such as show_sold_out & rooms can be used to show sold out rooms and all available rooms.\n            \nThe API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "hotels",
      "item": [
        {
          "id": "a659a8ce-86d9-4816-bf7d-1fb2f6be9689",
          "name": "getHotelsSearchBox",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/hotels/search-box?all_rooms=%7B%7D&amenity=%7B%7D&chain=%7B%7D&check_in=%7B%7D&check_out=%7B%7D&currency=%7B%7D&lang=%7B%7D&max_rate=%7B%7D&north_east_corner=%7B%7D&number_of_results=%7B%7D&show_sold_out=%7B%7D&south_west_corner=%7B%7D",
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
              "id": "e2fdfd20-1a4c-475f-b18a-d10a9c613bab"
            }
          ]
        }
      ]
    }
  ]
}