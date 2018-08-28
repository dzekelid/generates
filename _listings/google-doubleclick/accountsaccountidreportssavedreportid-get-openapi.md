---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get Saved Report
  version: 1.0.0
  description: Generate an Ad Exchange report based on the saved report ID sent in
    the query parameters.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/reports:
    get:
      summary: Get Reports
      description: Generate an Ad Exchange report based on the report request sent
        in the query parameters. Returns the result as JSON; to retrieve output in
        CSV format specify "alt=csv" as a query parameter.
      operationId: adexchangeseller.accounts.reports.generate
      x-api-path-slug: accountsaccountidreports-get
      parameters:
      - in: path
        name: accountId
        description: Account which owns the generated report
      - in: query
        name: dimension
        description: Dimensions to base the report on
      - in: query
        name: endDate
        description: End of the date range to report on in YYYY-MM-DD format, inclusive
      - in: query
        name: filter
        description: Filters to be run on the report
      - in: query
        name: locale
        description: Optional locale to use for translating report output to a local
          language
      - in: query
        name: maxResults
        description: The maximum number of rows of report data to return
      - in: query
        name: metric
        description: Numeric columns to include in the report
      - in: query
        name: sort
        description: The name of a dimension or metric to sort the resulting report
          on, optionally prefixed with + to sort ascending or - to sort descending
      - in: query
        name: startDate
        description: Start of the date range to report on in YYYY-MM-DD format, inclusive
      - in: query
        name: startIndex
        description: Index of the first row of report data to return
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /accounts/{accountId}/reports/{savedReportId}:
    get:
      summary: Get Saved Report
      description: Generate an Ad Exchange report based on the saved report ID sent
        in the query parameters.
      operationId: adexchangeseller.accounts.reports.saved.generate
      x-api-path-slug: accountsaccountidreportssavedreportid-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the saved report
      - in: query
        name: locale
        description: Optional locale to use for translating report output to a local
          language
      - in: query
        name: maxResults
        description: The maximum number of rows of report data to return
      - in: path
        name: savedReportId
        description: The saved report to retrieve
      - in: query
        name: startIndex
        description: Index of the first row of report data to return
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
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