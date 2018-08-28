---
swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 0
info:
  title: Jumpseller Get Countries Country Code Regions
  description: Retrieve all regions from a single country..
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /countries/{country_code}/regions.json:
    get:
      summary: Get Countries Country Code Regions
      description: Retrieve all regions from a single country..
      operationId: getCountriesCountryCodeRegions.json
      x-api-path-slug: countriescountry-coderegions-json-get
      parameters:
      - in: path
        name: country_code
        description: ISO3166 Country Code
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Countries
      - Country
      - Code
      - Regions
      - Json
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