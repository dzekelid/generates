---
swagger: "2.0"
x-collection-name: Trello
x-complete: 1
info:
  title: Trello
  description: this-document-describes-the-rest-api-of-trello-as-published-by-trello-com---a-hrefhttpstrello-comdocsindex-html-target-blankofficial-documentationa--a-hrefhttpstrello-comdocsapi-target-blankthe-html-pages-that-were-scraped-in-order-to-generate-this-specification-a
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/calendarKey/generate:
    post:
      summary: Post Boards Calendarkey Generate
      description: Post boards calendarkey generate.
      operationId: addBoardsCalendarKeyGenerateByIdBoard
      x-api-path-slug: boardsidboardcalendarkeygenerate-post
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Calendarkey
      - Generate
  /boards/{idBoard}/emailKey/generate:
    post:
      summary: Post Boards Emailkey Generate
      description: Post boards emailkey generate.
      operationId: addBoardsEmailKeyGenerateByIdBoard
      x-api-path-slug: boardsidboardemailkeygenerate-post
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Emailkey
      - Generate
---