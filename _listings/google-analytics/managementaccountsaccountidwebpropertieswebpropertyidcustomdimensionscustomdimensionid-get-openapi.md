---
swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 0
info:
  title: Google Analytics Get Custom Dimension
  description: Get a custom dimension to which the user has access.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /analytics/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customDimensions:
    get:
      summary: Get Custom Dimensions
      description: Lists custom dimensions to which the user has access.
      operationId: analytics.management.customDimensions.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdimensions-get
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom dimensions to retrieve
      - in: query
        name: max-results
        description: The maximum number of custom dimensions to include in this response
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimensions to retrieve
      responses:
        200:
          description: OK
      tags:
      - Dimension
    post:
      summary: Create Custom Dimension
      description: Create a new custom dimension.
      operationId: analytics.management.customDimensions.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdimensions-post
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom dimension to create
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimension to create
      responses:
        200:
          description: OK
      tags:
      - Dimension
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customDimensions/{customDimensionId}:
    get:
      summary: Get Custom Dimension
      description: Get a custom dimension to which the user has access.
      operationId: analytics.management.customDimensions.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdimensionscustomdimensionid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom dimension to retrieve
      - in: path
        name: customDimensionId
        description: The ID of the custom dimension to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimension to retrieve
      responses:
        200:
          description: OK
      tags:
      - Dimension
    patch:
      summary: Update Custom Dimensions
      description: Updates an existing custom dimension. This method supports patch
        semantics.
      operationId: analytics.management.customDimensions.patch
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdimensionscustomdimensionid-patch
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom dimension to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customDimensionId
        description: Custom dimension ID for the custom dimension to update
      - in: query
        name: ignoreCustomDataSourceLinks
        description: Force the update and ignore any warnings related to the custom
          dimension being linked to a custom data source / data set
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimension to update
      responses:
        200:
          description: OK
      tags:
      - Dimension
    put:
      summary: Update Custom Dimensions
      description: Updates an existing custom dimension.
      operationId: analytics.management.customDimensions.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustomdimensionscustomdimensionid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom dimension to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customDimensionId
        description: Custom dimension ID for the custom dimension to update
      - in: query
        name: ignoreCustomDataSourceLinks
        description: Force the update and ignore any warnings related to the custom
          dimension being linked to a custom data source / data set
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimension to update
      responses:
        200:
          description: OK
      tags:
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