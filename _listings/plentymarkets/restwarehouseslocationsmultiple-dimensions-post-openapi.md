---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Create multiple warehouse location dimensions
  description: Creates multiple warehouse location dimension.
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