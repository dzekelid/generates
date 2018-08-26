---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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
---