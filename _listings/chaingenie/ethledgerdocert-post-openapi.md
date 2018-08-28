---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Generate and Manage Document (Basic)
  description: "This is an over simplified version for testing this API for its powers
    a template - uses an inbuilt into ChainGenie template and values are preconfigured
    - just running this will work and provide you an IPFS handle to retrieve the document
    you generated with your variables / values from the template.\nUse an existing
    document on our server and generate a document with automated sign and routing
    to a recipient.  Ex. this configured api will generate a certificate for a student
    name (name) with the completed certificate course (course) and dated (date). \nThe
    document hash will be posted on blockchain and the actual document will be added
    to IPFS.  Want to retrieve your document? Check out the API - Write & Retrieve
    - Docs (IPFS)."
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ethledger/docert:
    post:
      summary: Generate and Manage Document (Basic)
      description: "This is an over simplified version for testing this API for its
        powers a template - uses an inbuilt into ChainGenie template and values are
        preconfigured - just running this will work and provide you an IPFS handle
        to retrieve the document you generated with your variables / values from the
        template.\nUse an existing document on our server and generate a document
        with automated sign and routing to a recipient.  Ex. this configured api will
        generate a certificate for a student name (name) with the completed certificate
        course (course) and dated (date). \nThe document hash will be posted on blockchain
        and the actual document will be added to IPFS.  Want to retrieve your document?
        Check out the API - Write & Retrieve - Docs (IPFS)."
      operationId: EthledgerDocertPost2
      x-api-path-slug: ethledgerdocert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: course
      - in: formData
        name: date
      - in: formData
        name: students
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Generate
      - Manage
      - Document
      - (Basic)
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