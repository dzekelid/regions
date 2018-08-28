---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Save or update a region alias
  version: 1.0.0
  description: Save or update a region alias.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/region/favourites:
    get:
      summary: Returns favorite regions
      description: Returns favorite regions.
      operationId: Region_GetAllFavourites
      x-api-path-slug: apiregionfavourites-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Favorite
      - Regions
  /api/region/favourites/{favouriteRegionId}:
    get:
      summary: Returns favorite regions
      description: Returns favorite regions.
      operationId: Region_GetFavouriteByfavouriteRegionId
      x-api-path-slug: apiregionfavouritesfavouriteregionid-get
      parameters:
      - in: path
        name: favouriteRegionId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Favorite
      - Regions
    delete:
      summary: Remove a region from your favourites
      description: Remove a region from your favourites.
      operationId: Region_RemoveFavouriteByfavouriteRegionId
      x-api-path-slug: apiregionfavouritesfavouriteregionid-delete
      parameters:
      - in: path
        name: favouriteRegionId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Region
      - From
      - Your
      - Favourites
  /api/region/{id}:
    get:
      summary: Gets a region by it's Id
      description: Gets a region by it's id.
      operationId: Region_GetByidBysource
      x-api-path-slug: apiregionid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: source
        description: Nation
      responses:
        200:
          description: OK
      tags:
      - S
      - Region
      - By
      - Its
      - Id
  /api/region/save:
    post:
      summary: Save region
      description: Save region.
      operationId: Region_SaveRegionByregionSaveCommand
      x-api-path-slug: apiregionsave-post
      parameters:
      - in: body
        name: regionSaveCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Region
  /api/region/alias/save:
    post:
      summary: Save or update a region alias
      description: Save or update a region alias.
      operationId: Region_SaveRegionAliasByregionAliasSaveCommand
      x-api-path-slug: apiregionaliassave-post
      parameters:
      - in: body
        name: regionAliasSaveCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Update
      - Region
      - Alias
  /api/region/{id}/nearby:
    get:
      summary: Gets the nearby regions for a region
      description: Gets the nearby regions for a region.
      operationId: Region_NearbyRegionsByid
      x-api-path-slug: apiregionidnearby-get
      parameters:
      - in: path
        name: id
        description: Id of the region
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Nearby
      - Regionsa
      - Region
  /api/region/favourites/add:
    post:
      summary: Add a region to your list of favourites
      description: Add a region to your list of favourites.
      operationId: Region_AddFavouriteBycommand
      x-api-path-slug: apiregionfavouritesadd-post
      parameters:
      - in: body
        name: command
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Region
      - To
      - Your
      - List
      - Of
      - Favourites
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