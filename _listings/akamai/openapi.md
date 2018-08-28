---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 1
info:
  title: Akamai API
  description: the-akamai-api-for-managing-your-akamai-service
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /config-media-security/v1/security/regions:
    get:
      summary: List Regions
      description: List Regions
      operationId: configmediasecurityv1securityregions
      x-api-path-slug: configmediasecurityv1securityregions-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Regions
  /config-media-security/v1/security/regions/{countryCode}:
    get:
      summary: List Regions per Country
      description: List Regions per Country
      operationId: configmediasecurityv1securityregionscountrycode
      x-api-path-slug: configmediasecurityv1securityregionscountrycode-get
      parameters:
      - in: query
        name: countryCode
        description: The country code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Regions
      - Countrycode
---