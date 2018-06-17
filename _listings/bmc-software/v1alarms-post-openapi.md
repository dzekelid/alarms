---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Create Alarm
  version: 1.0.0
  description: Create an Alarm
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
    post:
      summary: Create Alarm
      description: Create an Alarm
      operationId: create-alarm
      x-api-path-slug: v1alarms-post
      parameters:
      - in: formData
        name: name
        description: The name of the alarm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v1/alarm/:alarmId:
    get:
      summary: Get Alarm by Id
      description: Retrieves a single alarm
      operationId: get-alarm-by-id
      x-api-path-slug: v1alarmalarmid-get
      parameters:
      - in: query
        name: alarmId
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v1/alarms/search:
    get:
      summary: Get Alarms by Name
      description: Retrieves alarms by name
      operationId: get-alarms-by-name
      x-api-path-slug: v1alarmssearch-get
      parameters:
      - in: query
        name: alarmName
        type: string
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