---
swagger: "2.0"
info:
  title: Knoema API Dimension Group
  description: 'This endpoint used to list/add/edit/delete groups in dimensions. The
    functionality of endpoint depends on HTTP method: GET, POST, PUT or DELETE.'
  version: 1.0.0
host: knoema.com
basePath: /api/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /meta/group/{groupKey}:
    get:
      summary: Dimension Group
      description: This endpoint used to list/add/edit/delete groups in dimensions
      operationId: dimensionGroup
      responses:
        200:
          description: OK
      tags:
      - groups
      - dimensions
definitions: []
x-collection-name: Knoema
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