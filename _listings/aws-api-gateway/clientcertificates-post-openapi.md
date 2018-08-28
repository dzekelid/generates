---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 0
info:
  title: AWS API Gateway API Clientcertificate Generate
  version: 1.0.0
  description: Generates a new ClientCertificate resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /clientcertificates:
    post:
      summary: Clientcertificate Generate
      description: Generates a new ClientCertificate resource.
      operationId: clientcertificateGenerate
      x-api-path-slug: clientcertificates-post
      parameters:
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
      - Generate
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