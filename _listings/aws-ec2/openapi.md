swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeRegions:
    get:
      summary: Describe Regions
      description: Describes one or more regions that are currently available to you.
      operationId: describeregions
      x-api-path-slug: actiondescriberegions-get
      responses:
        200:
          description: OK
      tags:
      - Regions