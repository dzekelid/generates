---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Generate the warehouse location label
  description: Generates the warehouse location label
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/exports/generate_token:
    get:
      summary: Generate a token
      description: Creates a new token which can be used as <code>OutputParam</code>
        entry.
      operationId: getRestExportsGenerateToken
      x-api-path-slug: restexportsgenerate-token-get
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Token
  /rest/warehouses/locations/previews:
    post:
      summary: Generate warehouse location preview and saves it
      description: Generates warehouse location preview and saves it
      operationId: postRestWarehousesLocationsPreviews
      x-api-path-slug: restwarehouseslocationspreviews-post
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Warehouse
      - Location
      - Preview
      - Saves
      - It
  /rest/warehouses/locations/{warehouseId}/label:
    get:
      summary: Generate the warehouse location label
      description: Generates the warehouse location label
      operationId: getRestWarehousesLocationsWarehouseLabel
      x-api-path-slug: restwarehouseslocationswarehouseidlabel-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Warehouse
      - Location
      - Label
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