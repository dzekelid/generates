---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 1
info:
  title: Global Change Information System API
  description: who-we-are-what-the-gcis-is-and-how-we-use-identifiers-and-semantic-information-to-provide-points-of-reference-and-traceability--examples-and-tutorials-for-using-this-system-as-a-researcher-citizen-scientist-application-developer-or-information-theorist--a-description-of-how-the-information-is-structured-including-the-overlaps-between-relational-and-semantic-representations-of-the-information--complete-documentation-for-the-api-including-methods-for-browsing-and-finding-resources-
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /uuid:
    get:
      summary: Generate a UUID.
      description: <p>Generate version 4 Universally Unique Identifiers.  The algorithm
        used for thisn    is described <a target=_blank href=https://en.wikipedia.org/wiki/UUID#Version_4_.28random.29>here</a>.n    </p>
      operationId: pgenerate-version-4-universally-unique-identifiers--the-algorithm-used-for-this----is-described-a-ta
      x-api-path-slug: uuid-get
      parameters:
      - in: query
        name: count
        description: Number of UUIDs to generate (max 1000)
      responses:
        200:
          description: OK
      tags:
      - Generate
      - UUID
---