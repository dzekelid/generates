---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/promocode/generate:
    get:
      summary: Get Admin Promocode Generate
      description: Get admin promocode generate.
      operationId: getApiV1AdminPromocodeGenerate
      x-api-path-slug: apiv1adminpromocodegenerate-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
      - Generate
---