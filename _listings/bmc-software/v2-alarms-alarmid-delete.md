---
swagger: "2.0"
info:
  title: BMC Software API Delete Alarm
  version: 1.0.0
  description: Deletes an alarm
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/alarms/:alarmId:
    delete:
      summary: Delete Alarm
      description: Deletes an alarm
      operationId: delete-alarm
      parameters:
      - in: query
        name: |-
          alarmId
          The alarm to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - alarms
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