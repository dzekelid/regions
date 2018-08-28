---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: 'Entertainment Express '
  description: Get lineups by AreaID.
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /TvMedia/lineups/browse/{CountryID}/{RegionID}:
    get:
      summary: ""
      description: Get service areas for a specific country and region.
      operationId: GetTvMediaServiceAreas
      x-api-path-slug: tvmedialineupsbrowsecountryidregionid-get
      parameters:
      - in: path
        name: CountryID
        description: Country abbreviation
      - in: path
        name: RegionID
        description: Region abbreviation
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - Browse
      - CountryID
      - RegionID
  /TvMedia/lineups/browse/{CountryID}/{RegionID}/{AreaID}:
    get:
      summary: ""
      description: Get lineups by AreaID.
      operationId: GetTvMediaLineupsByAreaID
      x-api-path-slug: tvmedialineupsbrowsecountryidregionidareaid-get
      parameters:
      - in: path
        name: AreaID
        description: Service area ID
      - in: path
        name: CountryID
        description: Country abbreviation
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: LineupType
        description: Filter by lineup type, valid types are OTA, SAT, CAB, IPTV
      - in: query
        name: ProviderId
        description: Filter by provider ID
      - in: path
        name: RegionID
        description: Region abbreviation
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - Browse
      - CountryID
      - RegionID
      - AreaID
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