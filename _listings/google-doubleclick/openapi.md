---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 1
info:
  title: Google Doubleclick Merged API
  version: 1.0.0
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
---