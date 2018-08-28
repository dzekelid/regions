---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Get Regions Connector Image
  description: Generates connector-image url for the region. It requires the **administrator**
    role.
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /regions:
    get:
      summary: Get Regions
      description: Returns regions. It requires the **consumer** global role.
      operationId: FindRegions
      x-api-path-slug: regions-get
      parameters:
      - in: query
        name: query
        description: Filters the regions returned
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Regions
    post:
      summary: Post Regions
      description: Creates a new region.
      operationId: CreateRegion
      x-api-path-slug: regions-post
      parameters:
      - in: body
        name: region
        description: Add new region
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Regions
  /regions/{id}:
    delete:
      summary: Delete Regions
      description: Deletes a region
      operationId: Delete Region
      x-api-path-slug: regionsid-delete
      parameters:
      - in: query
        name: force
        description: Region may be in an odd state
      - in: path
        name: id
        description: ID of region to delete
      responses:
        200:
          description: OK
      tags:
      - Regions
    get:
      summary: Get Regions
      description: Returns a region based on its id. It requires the **consumer**
        global role.
      operationId: GetRegionById
      x-api-path-slug: regionsid-get
      parameters:
      - in: query
        name: discover
        description: will return child providers from aws
      - in: path
        name: id
        description: ID of region to fetch
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Regions
    patch:
      summary: Patch Regions
      description: Patches a region. PATCH only supports provider type(/rest/provider-types/ncs).
        Allowed fields to PATCH for NCS provider type are (name,location)
      operationId: PatchRegion
      x-api-path-slug: regionsid-patch
      parameters:
      - in: body
        name: body
        description: Patch region
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of region to patch
      responses:
        200:
          description: OK
      tags:
      - Regions
    put:
      summary: Put Regions
      description: Updates a region. **Not implemented**
      operationId: UpdateRegion
      x-api-path-slug: regionsid-put
      parameters:
      - in: path
        name: id
        description: ID of region to update
      - in: body
        name: region
        description: Update region
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Regions
  /regions/{id}/connection:
    delete:
      summary: Delete Regions Connection
      description: ""
      operationId: DeleteRegionConnection
      x-api-path-slug: regionsidconnection-delete
      parameters:
      - in: path
        name: id
        description: ID of region
      responses:
        200:
          description: OK
      tags:
      - Regions
      - Connection
    get:
      summary: Get Regions Connection
      description: Get region connection.
      operationId: GetRegionConnection
      x-api-path-slug: regionsidconnection-get
      parameters:
      - in: path
        name: id
        description: ID of region
      responses:
        200:
          description: OK
      tags:
      - Regions
      - Connection
    post:
      summary: Post Regions Connection
      description: Creates a new region connection
      operationId: CreateRegionConnection
      x-api-path-slug: regionsidconnection-post
      parameters:
      - in: path
        name: id
        description: ID of region
      - in: body
        name: regionConnection
        description: Add new region connection
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Regions
      - Connection
  /regions/{id}/connector-image:
    get:
      summary: Get Regions Connector Image
      description: Generates connector-image url for the region. It requires the **administrator**
        role.
      operationId: getConnectorImage
      x-api-path-slug: regionsidconnectorimage-get
      parameters:
      - in: path
        name: id
        description: ID of region to fetch the connector-image
      responses:
        200:
          description: OK
      tags:
      - Regions
      - Connector
      - Image
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