---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Position Regions
  description: Position all regions for a Layout
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /region/position/all/{layoutId}:
    put:
      summary: Position Regions
      description: Position all regions for a Layout
      operationId: regionPositionAll
      x-api-path-slug: regionpositionalllayoutid-put
      parameters:
      - in: path
        name: layoutId
        description: The Layout ID
      - in: formData
        name: regions
        description: Array of regions and their new positions
      responses:
        200:
          description: OK
      tags:
      - Position
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