---
swagger: "2.0"
x-collection-name: AWS CloudWatch
x-complete: 0
info:
  title: Amazon CloudWatch API Put Metric Alarm
  version: 1.0.0
  description: Creates or updates an alarm and associates it with the specified metric.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteAlarms:
    "":
      summary: Delete Alarms
      description: Deletes the specified alarms.
      operationId: deletealarms
      x-api-path-slug: actiondeletealarms-
      parameters:
      - in: query
        name: AlarmNames.member.N
        description: The alarms to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /?Action=DescribeAlarms:
    "":
      summary: Describe Alarms
      description: Retrieves the specified alarms.
      operationId: describealarms
      x-api-path-slug: actiondescribealarms-
      parameters:
      - in: query
        name: ActionPrefix
        description: The action name prefix
        type: string
      - in: query
        name: AlarmNamePrefix
        description: The alarm name prefix
        type: string
      - in: query
        name: AlarmNames.member.N
        description: The names of the alarms
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of alarm descriptions to retrieve
        type: string
      - in: query
        name: NextToken
        description: The token returned by a previous call to indicate that there
          is more dataavailable
        type: string
      - in: query
        name: StateValue
        description: The state value to be used in matching alarms
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /?Action=DisableAlarmActions:
    "":
      summary: Disable Alarm Actions
      description: Disables the actions for the specified alarms.
      operationId: disablealarmactions
      x-api-path-slug: actiondisablealarmactions-
      parameters:
      - in: query
        name: AlarmNames.member.N
        description: The names of the alarms
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarm Actions
  /?Action=EnableAlarmActions:
    "":
      summary: Enable Alarm Actions
      description: Enables the actions for the specified alarms.
      operationId: enablealarmactions
      x-api-path-slug: actionenablealarmactions-
      parameters:
      - in: query
        name: AlarmNames.member.N
        description: The names of the alarms
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarm Actions
  /?Action=DescribeAlarmHistory:
    "":
      summary: Describe Alarm History
      description: Retrieves the history for the specified alarm.
      operationId: describealarmhistory
      x-api-path-slug: actiondescribealarmhistory-
      parameters:
      - in: query
        name: AlarmName
        description: The name of the alarm
        type: string
      - in: query
        name: EndDate
        description: The ending date to retrieve alarm history
        type: string
      - in: query
        name: HistoryItemType
        description: The type of alarm histories to retrieve
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of alarm history records to retrieve
        type: string
      - in: query
        name: NextToken
        description: The token returned by a previous call to indicate that there
          is more dataavailable
        type: string
      - in: query
        name: StartDate
        description: The starting date to retrieve alarm history
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarm History
  /?Action=PutMetricAlarm:
    "":
      summary: Put Metric Alarm
      description: Creates or updates an alarm and associates it with the specified
        metric.
      operationId: putmetricalarm
      x-api-path-slug: actionputmetricalarm-
      parameters:
      - in: query
        name: ActionsEnabled
        description: Indicates whether actions should be executed during any changes
          to the alarm state
        type: string
      - in: query
        name: AlarmActions.member.N
        description: The actions to execute when this alarm transitions to the ALARM
          state from any other state
        type: string
      - in: query
        name: AlarmDescription
        description: The description for the alarm
        type: string
      - in: query
        name: AlarmName
        description: The name for the alarm
        type: string
      - in: query
        name: ComparisonOperator
        description: The arithmetic operation to use when comparing the specified
          statistic andthreshold
        type: string
      - in: query
        name: Dimensions.member.N
        description: The dimensions for the metric associated with the alarm
        type: string
      - in: query
        name: EvaluationPeriods
        description: The number of periods over which data is compared to the specifiedthreshold
        type: string
      - in: query
        name: ExtendedStatistic
        description: The percentile statistic for the metric associated with the alarm
        type: string
      - in: query
        name: InsufficientDataActions.member.N
        description: The actions to execute when this alarm transitions to the INSUFFICIENT_DATA
          state from any other state
        type: string
      - in: query
        name: MetricName
        description: The name for the metric associated with the alarm
        type: string
      - in: query
        name: Namespace
        description: The namespace for the metric associated with the alarm
        type: string
      - in: query
        name: OKActions.member.N
        description: The actions to execute when this alarm transitions to an OK statefrom
          any other state
        type: string
      - in: query
        name: Period
        description: The period, in seconds, over which the specified statistic is
          applied
        type: string
      - in: query
        name: Statistic
        description: The statistic for the metric associated with the alarm, other
          than percentile
        type: string
      - in: query
        name: Threshold
        description: The value against which the specified statistic is compared
        type: string
      - in: query
        name: Unit
        description: The unit of measure for the statistic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarm Metric
  /?Action=DescribeAlarmsForMetric:
    "":
      summary: Describe Alarms For Metric
      description: Retrieves the alarms for the specified metric.
      operationId: describealarmsformetric
      x-api-path-slug: actiondescribealarmsformetric-
      parameters:
      - in: query
        name: Dimensions.member.N
        description: The dimensions associated with the metric
        type: string
      - in: query
        name: ExtendedStatistic
        description: The percentile statistic for the metric
        type: string
      - in: query
        name: MetricName
        description: The name of the metric
        type: string
      - in: query
        name: Namespace
        description: The namespace of the metric
        type: string
      - in: query
        name: Period
        description: The period, in seconds, over which the statistic is applied
        type: string
      - in: query
        name: Statistic
        description: The statistic for the metric, other than percentiles
        type: string
      - in: query
        name: Unit
        description: The unit for the metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarm Metrics
  /?Action=SetAlarmState:
    "":
      summary: Set Alarm State
      description: Temporarily sets the state of an alarm for testing purposes.
      operationId: setalarmstate
      x-api-path-slug: actionsetalarmstate-
      parameters:
      - in: query
        name: AlarmName
        description: The name for the alarm
        type: string
      - in: query
        name: StateReason
        description: The reason that this alarm is set to this specific state, in
          text format
        type: string
      - in: query
        name: StateReasonData
        description: The reason that this alarm is set to this specific state, in
          JSON format
        type: string
      - in: query
        name: StateValue
        description: The value of the state
        type: string
      responses:
        200:
          description: OK
      tags:
      - Aler State
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