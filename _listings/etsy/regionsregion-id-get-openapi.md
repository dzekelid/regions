---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Get Regions Region
  description: Retrieves a Region by id.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---