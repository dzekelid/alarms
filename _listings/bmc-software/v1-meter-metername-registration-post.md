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
  /v1/meter/:meterName/registration:
    post:
      summary: Registration
      description: Register a Meter with TrueSight Pulse
      operationId: registration
      parameters:
      - in: formData
        name: meterVersion
        description: What version of the Meter is running, ex
        type: string
      responses:
        200:
          description: OK
      tags:
      - meters
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