---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get Dimensions
  version: 1.0.0
  description: List the metadata for the dimensions available to this AdExchange account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/metadata/dimensions:
    get:
      summary: Get Dimensions
      description: List the metadata for the dimensions available to this AdExchange
        account.
      operationId: adexchangeseller.accounts.metadata.dimensions.list
      x-api-path-slug: accountsaccountidmetadatadimensions-get
      parameters:
      - in: path
        name: accountId
        description: Account with visibility to the dimensions
      responses:
        200:
          description: OK
      tags:
      - Advertising
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