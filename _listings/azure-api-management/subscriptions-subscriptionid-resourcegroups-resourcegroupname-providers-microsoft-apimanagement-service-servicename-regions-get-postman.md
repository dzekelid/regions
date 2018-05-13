{
  "info": {
    "name": "Azure API Management API Regions ListByService",
    "_postman_id": "bb59c764-2e90-4035-bcc8-97f7ff5c5d19",
    "description": "Lists all azure regions in which the service exists.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "regions",
      "item": [
        {
          "id": "c9cffc94-88c6-42e6-8080-cd00a041d465",
          "name": "Regions_ListByService",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/regions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "serviceName",
                  "value": "serviceName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all azure regions in which the service exists"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5646e899-ec43-4697-bd3a-f321d64fd310"
            }
          ]
        }
      ]
    }
  ]
}