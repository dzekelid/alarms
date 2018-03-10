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
  /v1/hostgroups/:hostgroupId:
    delete:
      summary: Delete Hostgroup
      description: Delete an hostgroup
      operationId: delete-hostgroup
      parameters:
      - in: query
        name: |-
          hostgroupId
          The hostgroup to delete
          forceRemove
          Remove the hostgroup, even if it&#39;s being used by a dashboard or alarm
        type: string
      responses:
        200:
          description: OK
      tags:
      - hostgroups
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