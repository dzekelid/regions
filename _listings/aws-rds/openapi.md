swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
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
        region can create a Read Replica \n            or copy a DB snapshot from."
      operationId: describesourceregions
      x-api-path-slug: actiondescribesourceregions-get
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
      - Source Regions