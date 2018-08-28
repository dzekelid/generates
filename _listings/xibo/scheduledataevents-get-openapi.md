---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Generates the calendar that we draw events on
  description: ""
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /schedule/data/events:
    get:
      summary: Generates the calendar that we draw events on
      description: ""
      operationId: scheduleCalendarData
      x-api-path-slug: scheduledataevents-get
      parameters:
      - in: formData
        name: displayGroupIds
        description: The DisplayGroupIds to return the schedule for
      - in: formData
        name: from
        description: From Date Timestamp in Microseconds
      - in: formData
        name: to
        description: To Date Timestamp in Microseconds
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Calendar
      - That
      - We
      - Draw
      - Events
      - "On"
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