swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/mfa/generate:
    post:
      summary: Generate MFA secret
      description: |-
        Generates an multi-factor authentication secret for a user and returns it as a string and as base64 encoded QR code image.
        ##### Permissions
        Must be logged in as the user or have the `edit_other_users` permission.
      operationId: generates-an-multifactor-authentication-secret-for-a-user-and-returns-it-as-a-string-and-as-base64-e
      x-api-path-slug: usersuser-idmfagenerate-post
      parameters:
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Generate
      - MFA
      - Secret
  /commands/{command_id}/regen_token:
    put:
      summary: Generate a new token
      description: |-
        Generate a new token for the command based on command id string.
        ##### Permissions
        Must have `manage_slash_commands` permission for the team the command is in.
      operationId: generate-a-new-token-for-the-command-based-on-command-id-string-permissionsmust-have-manage-slash-co
      x-api-path-slug: commandscommand-idregen-token-put
      parameters:
      - in: path
        name: command_id
        description: ID of the command to generate the new token
      responses:
        200:
          description: OK
      tags:
      - Generate
      - New
      - Token