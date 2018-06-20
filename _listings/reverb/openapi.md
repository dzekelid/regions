---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shipping/regions:
    get:
      summary: Get Shipping Regions
      description: Get shipping regions.
      operationId: getShippingRegions
      x-api-path-slug: shippingregions-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Regions
---