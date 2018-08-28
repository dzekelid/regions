{
  "info": {
    "name": "Plentymarkets Lists parcel service regions by parcel service preset id.",
    "_postman_id": "0c6a7cfd-3cef-44bf-a12f-8d8abd75d8ff",
    "description": "Lists parcel service regions. The ID of the parcel service preset must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "67a7d7f6-95ad-4b32-a3d5-79bc119eeb34",
          "name": "getRestOrdersShippingPresetsPresetParcelServiceRegions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/shipping/presets/:presetId/parcel_service_regions"
              ],
              "query": [
                {
                  "key": "$parcelServicePresetId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "columns",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "presetId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists parcel service regions. The ID of the parcel service preset must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "581c3f33-b6a3-4a9e-9d2b-a89405f54ea8"
            }
          ]
        }
      ]
    }
  ]
}