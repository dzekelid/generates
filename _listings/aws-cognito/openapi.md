---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetId:
    get:
      summary: Get Id
      description: Generates (or retrieves) a Cognito ID.
      operationId: getId
      x-api-path-slug: actiongetid-get
      parameters:
      - in: query
        name: AccountId
        description: A standard AWS account ID (9+ digits)
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: Logins
        description: A set of optional name-value pairs that map provider names to
          provider tokens
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identities
---