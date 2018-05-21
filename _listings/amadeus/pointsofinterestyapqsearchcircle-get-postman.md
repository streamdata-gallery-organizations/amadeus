{
  "info": {
    "name": "Amadeus Get Points Of Interest Yapq Search Circle",
    "_postman_id": "2cebce7f-4782-4fe8-a873-dfc3f6c0684f",
    "description": "Amadeus has partnered with YapQ to bring you point of interest APIs with the goal of offering you unbiased ratings of landmarks and tourist attractions. YapQ rates places according to their interest on social media and provides Wikipedia content and Geonames ID at a given location. \nYapQ's service indexes millions of points around the world, and provides content in 12 different languages. This allows you to ensure you catch the must-see sights at a specific YapQ supported location.\nEach point of interest comes with links to content, grading information, location and directions to help make discovering your destination easy and fun.\nThis service is still under active development, and the response format may change without warning. We'd be interested in your feedback - send us an email.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "points",
      "item": [
        {
          "id": "422fabb0-24b7-40d7-bdcd-8927329401fe",
          "name": "getPointsOfInterestYapqSearchCircle",
          "request": {
            "url": "http://api.sandbox.amadeus.com/v1.2/points-of-interest/yapq-search-circle?category=%7B%7D&geonames=%7B%7D&image_size=%7B%7D&lang=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&number_of_images=%7B%7D&number_of_results=%7B%7D&radius=%7B%7D&social_media=%7B%7D&vibes=%7B%7D",
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
              "id": "3562bc8c-166f-4e4c-89c0-89eebf265a44"
            }
          ]
        }
      ]
    }
  ]
}