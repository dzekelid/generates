---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 1
info:
  title: AWS API Gateway API
  version: 1.0.0
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
---