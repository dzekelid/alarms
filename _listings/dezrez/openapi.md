swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/property/{id}/alarms/add:
    post:
      summary: Add alarm codes for a property
      description: Add alarm codes for a property.
      operationId: Property_AddAlarmsByidByalarmsToAdd
      x-api-path-slug: apipropertyidalarmsadd-post
      parameters:
      - in: body
        name: alarmsToAdd
        description: A collection of alarm codes to add
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Alarm
      - Codesa
      - Property
  /api/property/{id}/alarms/remove:
    delete:
      summary: Remove alarm codes from a property
      description: Remove alarm codes from a property.
      operationId: Property_RemoveAlarmsByidByalarmIds
      x-api-path-slug: apipropertyidalarmsremove-delete
      parameters:
      - in: query
        name: alarmIds
        description: The ids of the alarm codes to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Alarm
      - Codes
      - From
      - Property
  /api/property/{id}/alarms:
    get:
      summary: Get a list of alarms for a property
      description: Get a list of alarms for a property.
      operationId: Property_AlarmsByid
      x-api-path-slug: apipropertyidalarms-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Alarmsa
      - Property