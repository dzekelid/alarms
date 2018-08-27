---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Core API Base station alarms retrieval
  description: Retrieves a list of base station alarms existing within authorized
    scopes. Note that in case of an OPERATOR scope, only supplier-owned base station
    alarms are returned.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /core/v141/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /deviceAlarms:
    get:
      summary: Device alarms retrieval
      description: Retrieves a list of device alarms existing within authorized scopes.
      operationId: retrieves-a-list-of-device-alarms-existing-within-authorized-scopes
      x-api-path-slug: devicealarms-get
      parameters:
      - in: query
        name: deviceEUI
        description: EUI of the device to search alarms for
      - in: query
        name: pageIndex
        description: If set, enables pagination and returns only the 100 device alarms
          of the specified page
      responses:
        200:
          description: OK
      tags:
      - Device
      - Alarms
      - Retrieval
  /baseStationAlarms:
    get:
      summary: Base station alarms retrieval
      description: Retrieves a list of base station alarms existing within authorized
        scopes. Note that in case of an OPERATOR scope, only supplier-owned base station
        alarms are returned.
      operationId: retrieves-a-list-of-base-station-alarms-existing-within-authorized-scopes-note-that-in-case-of-an-op
      x-api-path-slug: basestationalarms-get
      parameters:
      - in: query
        name: baseStationId
        description: Id of the base station to search alarms for
      - in: query
        name: pageIndex
        description: If set, enables pagination and returns only the 100 base station
          alarms of the specified page
      responses:
        200:
          description: OK
      tags:
      - Base
      - Station
      - Alarms
      - Retrieval
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