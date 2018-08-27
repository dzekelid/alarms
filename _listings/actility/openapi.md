swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
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
  /deviceAlarms/{deviceAlarmRef}:
    get:
      summary: Device alarm retrieval
      description: Retrieves the device alarm corresponding to the provided device
        alarm ref, if that device alarm is within authorized scopes.
      operationId: retrieves-the-device-alarm-corresponding-to-the-provided-device-alarm-ref-if-that-device-alarm-is-wi
      x-api-path-slug: devicealarmsdevicealarmref-get
      parameters:
      - in: path
        name: deviceAlarmRef
        description: Ref of the device alarm to retrieve
      responses:
        200:
          description: OK
      tags:
      - Device
      - Alarm
      - Retrieval
  /deviceAlarms/{deviceAlarmRef}/acks:
    post:
      summary: Device alarm acknowledgement
      description: Acknowledges a device alarm.
      operationId: acknowledges-a-device-alarm
      x-api-path-slug: devicealarmsdevicealarmrefacks-post
      parameters:
      - in: path
        name: deviceAlarmRef
        description: Ref of the device alarm to acknowledge
      responses:
        200:
          description: OK
      tags:
      - Device
      - Alarm
      - Acknowledgement
  /baseStationAlarms/{baseStationAlarmRef}:
    get:
      summary: Base station alarm retrieval
      description: Retrieves the base station alarm corresponding to the provided
        base station alarm ref, if that base station alarm is within authorized scopes.
      operationId: retrieves-the-base-station-alarm-corresponding-to-the-provided-base-station-alarm-ref-if-that-base-s
      x-api-path-slug: basestationalarmsbasestationalarmref-get
      parameters:
      - in: path
        name: baseStationAlarmRef
        description: Ref of the base station alarm to retrieve
      responses:
        200:
          description: OK
      tags:
      - Base
      - Station
      - Alarm
      - Retrieval
  /baseStationAlarms/{baseStationAlarmRef}/acks:
    post:
      summary: Base station alarm acknowledgement
      description: Acknowledges a base station alarm.
      operationId: acknowledges-a-base-station-alarm
      x-api-path-slug: basestationalarmsbasestationalarmrefacks-post
      parameters:
      - in: path
        name: baseStationAlarmRef
        description: Ref of the base station alarm to acknowledge
      responses:
        200:
          description: OK
      tags:
      - Base
      - Station
      - Alarm
      - Acknowledgement