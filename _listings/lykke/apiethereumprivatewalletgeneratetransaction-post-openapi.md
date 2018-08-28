---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Ethereum Privatewallet Generatetransaction
  version: 1.0.0
  description: Add api ethereum privatewallet generatetransaction.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Ethereum/privateWallet/generateTransaction:
    post:
      summary: Add API Ethereum Privatewallet Generatetransaction
      description: Add api ethereum privatewallet generatetransaction.
      operationId: ApiEthereumPrivateWalletGenerateTransactionPost
      x-api-path-slug: apiethereumprivatewalletgeneratetransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Privatewallet
      - Generatetransaction
  /api/GenerateTransferTransaction:
    post:
      summary: Add API Generatetransfertransaction
      description: Add api generatetransfertransaction.
      operationId: ApiGenerateTransferTransactionPost
      x-api-path-slug: apigeneratetransfertransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Generatetransfertransaction
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