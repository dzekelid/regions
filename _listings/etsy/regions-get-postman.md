{
  "info": {
    "name": "Etsy Get Regions",
    "_postman_id": "f65278f3-9ac3-41aa-9325-a4c82f8c4b56",
    "description": "Finds all Region.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Regions",
      "item": [
        {
          "id": "f9109659-0300-46b8-868b-115d2fd6b54d",
          "name": "getRegionsRegion",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "regions/:region_id"
              ],
              "variable": [
                {
                  "id": "region_id",
                  "value": "region_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Region by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0105b4e7-6fa5-4acf-8c81-2ad742252b32"
            }
          ]
        },
        {
          "id": "30acbfc9-37f7-4b1c-9914-d9a397fa4706",
          "name": "getRegions",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/regions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all Region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "439ae5a4-57f3-409d-93d1-30e7e7f3df29"
            }
          ]
        }
      ]
    }
  ]
}