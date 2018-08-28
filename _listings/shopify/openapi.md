swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/gift_cards.json:
    post:
      summary: Create a new gift card with an automatically generated code
      description: Create a new gift card with an automatically generated code.
      operationId: postAdminGiftCards.json
      x-api-path-slug: admingift-cards-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Gift
      - Card
      - Automatically
      - Generated
      - Code