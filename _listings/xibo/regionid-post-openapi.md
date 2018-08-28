---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Add Region
  description: Add a Region to a Layout
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
  /region/{id}:
    put:
      summary: Edit Region
      description: Edit Region
      operationId: regionEdit
      x-api-path-slug: regionid-put
      parameters:
      - in: formData
        name: height
        description: The Height
      - in: path
        name: id
        description: The Region ID to Edit
      - in: formData
        name: left
        description: The Left Coordinate
      - in: formData
        name: loop
        description: Flag indicating whether this region should loop if there is only
          1 media item in the timeline
      - in: formData
        name: top
        description: The Top Coordinate
      - in: formData
        name: transitionDirection
        description: The transition direction if required by the transition type
      - in: formData
        name: transitionDuration
        description: The transition duration in milliseconds if required by the transition
          type
      - in: formData
        name: transitionType
        description: The Transition Type
      - in: formData
        name: width
        description: The Width, default 250
      - in: formData
        name: zIndex
        description: The Layer for this Region
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Region
    post:
      summary: Add Region
      description: Add a Region to a Layout
      operationId: regionAdd
      x-api-path-slug: regionid-post
      parameters:
      - in: formData
        name: height
        description: The Height
      - in: path
        name: id
        description: The Layout ID to add the Region to
      - in: formData
        name: left
        description: The Left Coordinate
      - in: formData
        name: top
        description: The Top Coordinate
      - in: formData
        name: width
        description: The Width, default 250
      responses:
        200:
          description: OK
      tags:
      - Region
  /region/{regionId}:
    delete:
      summary: Region Delete
      description: Delete an existing region
      operationId: regionDelete
      x-api-path-slug: regionregionid-delete
      parameters:
      - in: path
        name: regionId
        description: The Region ID to Delete
      responses:
        200:
          description: OK
      tags:
      - Region
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