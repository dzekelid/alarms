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
  /v1/metrics/dashactions/:dashboardSetId:
    get:
      summary: Get actions for a dashboard
      description: |2-
         Retrieves the needed configuration changes for a dashboard
         Returns an an array of objects, each has the following properties:
      operationId: get-actions-for-a-dashboard
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