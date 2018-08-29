{
  "info": {
    "name": "Amadeus Get Trains Schedule Search",
    "_postman_id": "8553bb0b-c839-4a98-848e-a039aa777f70",
    "description": "This API allows you to find all the possible destinations in the Rail Instant Search cache (used by Extensive Search above) from a given origin station on a given day. You can use this to help build network maps, journey planners or provide inspiration for rail travel.\n\nThis API has continuous content from SNCF.\nAll the options returned are single-leg trips - where a single train takes you directly from the origin to the destination. In general, only departure dates up to 90 days in the future are supported\n\nCurrently agglomeration stations are not supported",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "trains",
      "item": [
        {
          "id": "1df4e270-d143-4dac-9273-892b102e5a19",
          "name": "getTrainsScheduleSearch",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/trains/schedule-search?departure_date=%7B%7D&origin=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API allows you to find all the possible destinations in the Rail Instant Search cache (used by Extensive Search above) from a given origin station on a given day"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e8f0734-cccf-46d3-9a1f-2171fc46b555"
            }
          ]
        }
      ]
    }
  ]
}