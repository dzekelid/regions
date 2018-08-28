swagger: "2.0"
x-collection-name: AWS Rekognition
x-complete: 1
info:
  title: AWS Rekognition API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateCollection:
    get:
      summary: Create Collection
      description: Creates a collection in an AWS Region.
      operationId: createCollection
      x-api-path-slug: actioncreatecollection-get
      parameters:
      - in: query
        name: CollectionId
        description: ID for the collection that you are creating
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Collections