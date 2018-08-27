---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Get All Alarms
  version: 1.0.0
  description: Get all of the Alarms
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/alarms:
    get:
      summary: Get All Alarms
      description: Get all of the Alarms
      operationId: get-all-alarms
      x-api-path-slug: v1alarms-get
      responses:
        200:
          description: OK
      tags:
      - Alarms
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