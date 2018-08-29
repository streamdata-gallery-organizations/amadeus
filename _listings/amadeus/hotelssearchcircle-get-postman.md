{
  "info": {
    "name": "Amadeus Get Hotels Search Circle",
    "_postman_id": "6595be27-2354-4cc3-bf9a-197a55fe65b9",
    "description": "A fast Hotel shopping API to see which hotels are available in a given area, on a given day and displays their lowest prices. With this API you can find out the price of the cheapest daily rate for all hotels within a specified radius of a point.\n\nThis API allows you to quickly see the hotel locations in a region, and what prices in that area look like,  as well as the check-in and check-out dates, and get list of up to 140 properties (names, codes, image, amenities) with their locations and rates. Optional parameters such as currency and maximum rates, amenities or hotel chain codes are also available and can be used to narrow down the results. More optional parameters such as show_sold_out & rooms can be used to show sold out rooms and all available rooms. \n\nThe API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "hotels",
      "item": [
        {
          "id": "65abd19b-a536-4dbd-aaf6-815becd26b20",
          "name": "getHotelsSearchCircle",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/hotels/search-circle?all_rooms=%7B%7D&amenity=%7B%7D&chain=%7B%7D&check_in=%7B%7D&check_out=%7B%7D&currency=%7B%7D&lang=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&max_rate=%7B%7D&number_of_results=%7B%7D&radius=%7B%7D&show_sold_out=%7B%7D",
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
              "id": "71068a76-681f-42a2-9137-7fd4ce129d04"
            }
          ]
        }
      ]
    }
  ]
}