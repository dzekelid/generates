swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accessCodes:
    post:
      summary: Access code generation
      description: Generates a new access code. If it is of type 'userAccessCode',
        the provided userId must reference an user within authorized scopes. This
        access code can then be used to access the targetted application without re-typing
        credentials (ThingPark SSO). In order to do so, the code needs to be appended
        to the application portal URL, i.e. 'portalUrl?userAccessCode=code'.
      operationId: generates-a-new-access-code-if-it-is-of-type-useraccesscode-the-provided-userid-must-reference-an-us
      x-api-path-slug: accesscodes-post
      parameters:
      - in: body
        name: accessCode
        description: Information about the access code to generate
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Access
      - Code
      - Generation
  /appKeyGens:
    post:
      summary: AppKey generation
      description: Generate some encrypted VendorKeys with an HSM. Encrypted VendorKeys
        can be decrypted with the private part of provided RSA key. A VendorKey is
        a concatenation of an AppKey (128 bits) and hsmEncryptedAppKey (128 bits).
      operationId: generate-some-encrypted-vendorkeys-with-an-hsm-encrypted-vendorkeys-can-be-decrypted-with-the-privat
      x-api-path-slug: appkeygens-post
      parameters:
      - in: body
        name: appKeyGen
        description: Configuration for AppKey generation
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: number
        description: Define the number of AppKey generated
      responses:
        200:
          description: OK
      tags:
      - AppKey
      - Generation