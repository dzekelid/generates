swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
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