---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Lists parcel service regions by parcel service preset id.
  description: Lists parcel service regions. The ID of the parcel service preset must
    be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/orders/shipping/presets/{presetId}/parcel_service_regions:
    get:
      summary: Lists parcel service regions by parcel service preset id.
      description: Lists parcel service regions. The ID of the parcel service preset
        must be specified.
      operationId: getRestOrdersShippingPresetsPresetParcelServiceRegions
      x-api-path-slug: restordersshippingpresetspresetidparcel-service-regions-get
      parameters:
      - in: query
        name: $parcelServicePresetId
        description: The ID of the parcel service preset
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: presetId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Parcel
      - Service
      - Regions
      - By
      - Parcel
      - Service
      - Preset
      - Id
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