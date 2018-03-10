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
  '/custom_events/all?fromUtc={fromUtc}&amp;toUtc={toUtc} ':
    get:
      summary: Custom_events All?fromUtc={fromUtc}&amp;toUtc={toUtc}
      description: Gets all custom events using optional filter
      operationId: -custom-events-allfromutcfromutcamptoutctoutc-
      responses:
        200:
          description: OK
      tags:
      - custom events
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