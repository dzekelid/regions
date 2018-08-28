---
swagger: "2.0"
x-collection-name: AWS WAF
x-complete: 0
info:
  title: AWS WAF API Disassociate Web ACL
  version: 1.0.0
  description: 'Service: AWS WAF RegionalRemoves a web ACL from the specified resource.'
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssociateWebACL:
    get:
      summary: Associate Web ACL
      description: 'Service: AWS WAF RegionalAssociates a web ACL with a resource.'
      operationId: associateWebACL
      x-api-path-slug: actionassociatewebacl-get
      parameters:
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource to be protected
        type: string
      - in: query
        name: WebACLId
        description: A unique identifier (ID) for the web ACL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=DisassociateWebACL:
    get:
      summary: Disassociate Web ACL
      description: 'Service: AWS WAF RegionalRemoves a web ACL from the specified
        resource.'
      operationId: disassociateWebACL
      x-api-path-slug: actiondisassociatewebacl-get
      parameters:
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource from which the
          web ACL is being removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=GetWebACLForResource:
    get:
      summary: Get Web ACLFor Resource
      description: 'Service: AWS WAF RegionalReturns the web ACL for the specified
        resource.'
      operationId: getWebACLForResource
      x-api-path-slug: actiongetwebaclforresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource for which to get
          the web ACL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=ListResourcesForWebACL:
    get:
      summary: List Resources For Web ACL
      description: 'Service: AWS WAF RegionalReturns an array of resources associated
        with the specified web ACL.'
      operationId: listResourcesForWebACL
      x-api-path-slug: actionlistresourcesforwebacl-get
      parameters:
      - in: query
        name: WebACLId
        description: The unique identifier (ID) of the web ACL for which to list the
          associated resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
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