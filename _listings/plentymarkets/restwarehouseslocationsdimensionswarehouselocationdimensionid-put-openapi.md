---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update a warehouse location dimension
  description: Updates a warehouse location dimension
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
  /rest/warehouses/locations/multiple_dimensions:
    post:
      summary: Create multiple warehouse location dimensions
      description: Creates multiple warehouse location dimension.
      operationId: postRestWarehousesLocationsMultipleDimensions
      x-api-path-slug: restwarehouseslocationsmultiple-dimensions-post
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Warehouse
      - Location
      - Dimensions
  /rest/warehouses/{warehouseId}/locations/dimensions:
    get:
      summary: List warehouse location dimensions
      description: Lists all warehouse location dimensions.
      operationId: getRestWarehousesWarehouseLocationsDimensions
      x-api-path-slug: restwarehouseswarehouseidlocationsdimensions-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
      - Location
      - Dimensions
  /rest/warehouses/locations/dimensions:
    post:
      summary: Create a warehouse location dimension
      description: Creates a warehouse location dimension.
      operationId: postRestWarehousesLocationsDimensions
      x-api-path-slug: restwarehouseslocationsdimensions-post
      parameters:
      - in: query
        name: isActiveForPickupPath
        description: Active flag for pickup path of the warehouse location dimension
      - in: query
        name: level
        description: The level of the warehouse location dimension
      - in: query
        name: name
        description: The name of the warehouse location dimension
      - in: query
        name: parentId
        description: The parent ID of the warehouse location dimension
      - in: query
        name: separator
        description: The separator of the warehouse location dimension
      - in: query
        name: shortcut
        description: The shortcut of the warehouse location dimension
      - in: query
        name: warehouseId
        description: The warehouse ID of the warehouse location dimension
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Dimension
  /rest/warehouses/locations/dimensions/{warehouseLocationDimensionId}:
    delete:
      summary: Delete a warehouse location dimension
      description: Deletes a warehouse location dimension
      operationId: deleteRestWarehousesLocationsDimensionsWarehouselocationdimension
      x-api-path-slug: restwarehouseslocationsdimensionswarehouselocationdimensionid-delete
      parameters:
      - in: path
        name: warehouseLocationDimensionId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Dimension
    get:
      summary: Get a warehouse location dimension
      description: Gets a warehouse location dimension by ID. The warehouse location
        ID is required.
      operationId: getRestWarehousesLocationsDimensionsWarehouselocationdimension
      x-api-path-slug: restwarehouseslocationsdimensionswarehouselocationdimensionid-get
      parameters:
      - in: path
        name: warehouseLocationDimensionId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Dimension
    put:
      summary: Update a warehouse location dimension
      description: Updates a warehouse location dimension
      operationId: putRestWarehousesLocationsDimensionsWarehouselocationdimension
      x-api-path-slug: restwarehouseslocationsdimensionswarehouselocationdimensionid-put
      parameters:
      - in: path
        name: warehouseLocationDimensionId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Dimension
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