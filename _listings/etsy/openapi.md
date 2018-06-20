---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 1
info:
  title: Etsy
  description: bring-etsys-handmade-marketplace-and-community-into-your-apps-
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /regions/{region_id}:
    get:
      summary: Get Regions Region
      description: Retrieves a Region by id.
      operationId: getRegionsRegion
      x-api-path-slug: regionsregion-id-get
      parameters:
      - in: path
        name: region_id
      responses:
        200:
          description: OK
      tags:
      - Regions
      - Region
  /regions:
    get:
      summary: Get Regions
      description: Finds all Region.
      operationId: getRegions
      x-api-path-slug: regions-get
      responses:
        200:
          description: OK
      tags:
      - Regions
---