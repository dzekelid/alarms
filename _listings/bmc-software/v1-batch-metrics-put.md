---
swagger: "2.0"
info:
  title: BMC Software Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/batch/metrics:
    put:
      summary: Update metrics batch
      description: Updates a batch of metrics
      operationId: update-metrics-batch
      parameters:
      - in: formData
        name: |-
          type
          Type of metric, could be a device metric, a plugin metric or any arbitrary type
        description: |-
          description
          Description of the metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - batch
definitions: []
x-collection-name: BMC Software
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