---
swagger: "2.0"
x-collection-name: DonorsChoose
x-complete: 0
info:
  title: Donors Choose Generate Gift Code
  description: Generate Gift Code
  termsOfService: http://www.donorschoose.org/help/user_agreement.html
  version: "1"
host: api.donorschoose.org
basePath: common/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /json_api.html:
    post:
      summary: Generate Gift Code
      description: Generate Gift Code
      operationId: generate-gift-code
      x-api-path-slug: json-api-html-post
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Gift
      - Code
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