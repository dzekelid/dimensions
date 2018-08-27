---
swagger: "2.0"
x-collection-name: PredictHQ
x-complete: 0
info:
  title: PredictHQ Retrieve All Dimensions
  description: This action returns a summary for each dimension of your Signal.
  version: 1.0.0
host: api.predicthq.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/signals/{signal_id}/dimensions/:
    get:
      summary: Retrieve All Dimensions
      description: This action returns a summary for each dimension of your Signal.
      operationId: V1SignalsDimensionsBySignalIdGet
      x-api-path-slug: v1signalssignal-iddimensions-get
      parameters:
      - in: path
        name: signal_id
      responses:
        200:
          description: OK
      tags:
      - Signals
      - Signal
      - Dimensions
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---