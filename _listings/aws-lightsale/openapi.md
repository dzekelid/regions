---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 1
info:
  title: AWS Lightsale API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetRegions:
    get:
      summary: Get Regions
      description: Returns a list of all valid regions for Amazon Lightsail.
      operationId: getRegions
      x-api-path-slug: actiongetregions-get
      parameters:
      - in: query
        name: includeAvailabilityZones
        description: A Boolean value indicating whether to also include Availability
          Zones in your get      regions request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Regions
---