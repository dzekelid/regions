---
swagger: "2.0"
info:
  title: Amazon RDS API Describe Source Regions
  version: 1.0.0
  description: "Returns a list of the source AWS regions where the current AWS region
    can create a Read Replica \n            or copy a DB snapshot from."
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeSourceRegions:
    get:
      summary: Describe Source Regions
      description: "Returns a list of the source AWS regions where the current AWS
        region can create a Read Replica \n            or copy a DB snapshot from"
      operationId: describesourceregions
      parameters:
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous DescribeSourceRegions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: RegionName
        description: The source region name
        type: string
      responses:
        200:
          description: OK
      tags:
      - source regions
definitions: []
x-collection-name: AWS RDS
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