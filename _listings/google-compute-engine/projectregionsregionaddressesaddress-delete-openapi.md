---
swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 0
info:
  title: Google Compute Engine API Delete Region Address
  description: Deletes the specified address resource.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/regions:
    get:
      summary: Get Regions
      description: Retrieves the list of region resources available to the specified
        project.
      operationId: compute.regions.list
      x-api-path-slug: projectregions-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Region
  /{project}/regions/{region}:
    get:
      summary: Get Region
      description: Returns the specified Region resource. Get a list of available
        regions by making a list() request.
      operationId: compute.regions.get
      x-api-path-slug: projectregionsregion-get
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region resource to return
      responses:
        200:
          description: OK
      tags:
      - Region
  /{project}/regions/{region}/addresses:
    get:
      summary: Get Region Addresses
      description: Retrieves a list of addresses contained within the specified region.
      operationId: compute.addresses.list
      x-api-path-slug: projectregionsregionaddresses-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region for this request
      responses:
        200:
          description: OK
      tags:
      - Region Address
    post:
      summary: Create Region Address
      description: Creates an address resource in the specified project using the
        data included in the request.
      operationId: compute.addresses.insert
      x-api-path-slug: projectregionsregionaddresses-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region for this request
      responses:
        200:
          description: OK
      tags:
      - Region Address
  /{project}/regions/{region}/addresses/{address}:
    delete:
      summary: Delete Region Address
      description: Deletes the specified address resource.
      operationId: compute.addresses.delete
      x-api-path-slug: projectregionsregionaddressesaddress-delete
      parameters:
      - in: path
        name: address
        description: Name of the address resource to delete
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region for this request
      responses:
        200:
          description: OK
      tags:
      - Region Address
    get:
      summary: Get Region Address
      description: Returns the specified address resource.
      operationId: compute.addresses.get
      x-api-path-slug: projectregionsregionaddressesaddress-get
      parameters:
      - in: path
        name: address
        description: Name of the address resource to return
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region for this request
      responses:
        200:
          description: OK
      tags:
      - Region Address
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