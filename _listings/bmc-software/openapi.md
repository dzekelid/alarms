swagger: "2.0"
x-collection-name: BMC Software
x-complete: 1
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
    put:
      summary: Update Alarm
      description: Update an Alarm
      operationId: update-alarm
      x-api-path-slug: v1alarmalarmid-put
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
    delete:
      summary: Delete Alarm
      description: Deletes an alarm
      operationId: delete-alarm
      x-api-path-slug: v1alarmalarmid-delete
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
  /v2/alarms:
    post:
      summary: Create Alarm
      description: Create an Alarm
      operationId: create-alarm
      x-api-path-slug: v2alarms-post
      responses:
        200:
          description: OK
      tags:
      - Alarms
    get:
      summary: Get All Alarms
      description: Get all of the Alarms
      operationId: get-all-alarms
      x-api-path-slug: v2alarms-get
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v2/alarms/:alarmId:
    put:
      summary: Update Alarm
      description: Updates an alarm
      operationId: update-alarm
      x-api-path-slug: v2alarmsalarmid-put
      parameters:
      - in: query
        name: |-
          alarmId integer
          The alarm to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
    get:
      summary: Get Alarm by Id
      description: Retrieves a single alarm
      operationId: get-alarm-by-id
      x-api-path-slug: v2alarmsalarmid-get
      parameters:
      - in: query
        name: alarmId
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
    delete:
      summary: Delete Alarm
      description: Deletes an alarm
      operationId: delete-alarm
      x-api-path-slug: v2alarmsalarmid-delete
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
      - Alarms