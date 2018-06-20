---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /system/regions/:
    get:
      summary: Get System Regions
      description: |-
        Returns a single page response with a key of regions,
        containing a list of regions.
      operationId: getSystemRegions
      x-api-path-slug: systemregions-get
      responses:
        200:
          description: OK
      tags:
      - System
      - Regions
---