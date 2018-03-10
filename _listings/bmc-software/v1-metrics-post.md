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
  /v1/metrics:
    post:
      summary: Create metric
      description: Creates a new metric
      operationId: create-metric
      parameters:
      - in: formData
        name: |-
          name
          Name of the metric, must be globally unique, recommended that you add your own namespace
        description: |-
          type
          Type of metric, could be a device metric, a plugin metric or any arbitrary type
        type: string
      responses:
        200:
          description: OK
      tags:
      - metrics
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