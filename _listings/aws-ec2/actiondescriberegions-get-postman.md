{
  "info": {
    "name": "AWS EC2 API Describe Regions",
    "_postman_id": "65a3e734-e814-4991-a7b3-b8fc2c5d544e",
    "description": "Describes one or more regions that are currently available to you.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Regions",
      "item": [
        {
          "id": "272e4def-40e9-4563-8824-580aee1cb3f0",
          "name": "describeregions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRegions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more regions that are currently available to you."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f606a424-06f5-46e5-b1ab-25ade9a5664b"
            }
          ]
        }
      ]
    }
  ]
}