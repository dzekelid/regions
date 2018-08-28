swagger: "2.0"
x-collection-name: AWS WAF
x-complete: 1
info:
  title: AWS WAF API
  version: 1.0.0
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