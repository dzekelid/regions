{
  "info": {
    "name": "Youtube Get Regions",
    "_postman_id": "1788ebc3-2319-4c56-b875-7fc43aefc13d",
    "description": "Returns a list of content regions that the YouTube website supports.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "regions",
      "item": [
        {
          "id": "1b0bd4a8-14b7-487e-95fb-7bc84c0bdf52",
          "name": "getI18nregions",
          "request": {
            "url": "http://www.googleapis.com/youtube/v1/i18nRegions?hl=%7B%7D&part=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of content regions that the YouTube website supports"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0649f36-01a6-4d03-96e5-4e80fb7230fa"
            }
          ]
        }
      ]
    }
  ]
}