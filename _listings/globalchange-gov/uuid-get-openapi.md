---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API Generate a UUID.
  description: <p>Generate version 4 Universally Unique Identifiers.  The algorithm
    used for thisn    is described <a target=_blank href=https://en.wikipedia.org/wiki/UUID#Version_4_.28random.29>here</a>.n    </p>
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /uuid:
    get:
      summary: Generate a UUID.
      description: <p>Generate version 4 Universally Unique Identifiers.  The algorithm
        used for thisn    is described <a target=_blank href=https://en.wikipedia.org/wiki/UUID#Version_4_.28random.29>here</a>.n    </p>
      operationId: pgenerate-version-4-universally-unique-identifiers--the-algorithm-used-for-this----is-described-a-ta
      x-api-path-slug: uuid-get
      parameters:
      - in: query
        name: count
        description: Number of UUIDs to generate (max 1000)
      responses:
        200:
          description: OK
      tags:
      - Generate
      - UUID
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