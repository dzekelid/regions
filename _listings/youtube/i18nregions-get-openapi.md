---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Get Regions
  description: Returns a list of content regions that the YouTube website supports.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /i18nRegions:
    get:
      summary: Get Regions
      description: Returns a list of content regions that the YouTube website supports.
      operationId: getI18nregions
      x-api-path-slug: i18nregions-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter specifies the language that should be used for
          text values in the API response
      - in: query
        name: part
        description: The part parameter specifies the i18nRegion resource properties
          that the API response will include
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