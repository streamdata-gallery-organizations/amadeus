{
  "info": {
    "name": "Amadeus Get Points Of Interest Yapq Search Text",
    "_postman_id": "7f77d973-6bef-4f67-b5f5-a5dc76ba5064",
    "description": "Amadeus has partnered with YapQ to bring you point of interest APIs with the goal of offering you unbiased ratings of landmarks and tourist attractions. YapQ rates these points according to their interest on social media and provides Wikipedia content and Geonames ID in a given city. \nYapQ's service indexes millions of points around the world, and provides content in 12 different languages. This allows you to ensure you catch the must-see sights in a YapQ supported city.\nEach point of interest comes with links to content, grading information, location and directions to help make discovering your destination easy and fun.\nThis service is still under active development, and the response format may change without warning. We'd be interested in your feedback - send us an email.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "points",
      "item": [
        {
          "id": "9ccb0884-617f-4e30-b1e3-19374e7fdb06",
          "name": "getPointsOfInterestYapqSearchText",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/points-of-interest/yapq-search-text?category=%7B%7D&city_name=%7B%7D&geonames=%7B%7D&image_size=%7B%7D&lang=%7B%7D&number_of_images=%7B%7D&number_of_results=%7B%7D&social_media=%7B%7D&vibes=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Amadeus has partnered with YapQ to bring you point of interest APIs with the goal of offering you unbiased ratings of landmarks and tourist attractions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a6bcceb-66e0-4327-a0fa-e0bed4b44f7a"
            }
          ]
        }
      ]
    }
  ]
}