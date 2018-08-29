{
  "info": {
    "name": "Amadeus Get Hotels Property Code",
    "_postman_id": "d6a74940-e372-4986-8d47-51426f7068a6",
    "description": "This API allows you to quickly see the detailed information of a single hotel, including descriptions, address, GPS location, amenities, awards, lowest priced room and all room prices and booking information. \n\nThis API gives you more information on a specific property. Optional parameters such as show_sold_out & rooms can be used to show sold out rooms and all available rooms. \n\nThe API is based on our high-speed hotel pricing cache, which is also used to power the Amadeus Hotel Search Engine application. Results are returned very quickly, response times are generally under 2s. Our cache has great global coverage and is constantly refreshed with the latest prices.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "hotels",
      "item": [
        {
          "id": "307d1c84-b801-48c5-8921-5fa2b343ecad",
          "name": "getHotelsPropertyCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sandbox.amadeus.com",
              "path": [
                "v1.2",
                "hotels/:property_code"
              ],
              "query": [
                {
                  "key": "all_rooms",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "check_in",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "check_out",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "currency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lang",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "show_sold_out",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "property_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API allows you to quickly see the detailed information of a single hotel, including descriptions, address, GPS location, amenities, awards, lowest priced room and all room prices and booking information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8be70097-48f7-4e65-86f0-efb9638e2a4d"
            }
          ]
        }
      ]
    }
  ]
}