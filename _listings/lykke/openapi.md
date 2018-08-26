---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
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
---