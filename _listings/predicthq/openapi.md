---
swagger: "2.0"
x-collection-name: PredictHQ
x-complete: 1
info:
  title: PredictHQ API
  description: todo-add-description
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
---