---
name: Actility
x-slug: actility
description: 'Actility is the leader in low power wide area (LoRaWAN and 3GPP) network
  connectivity management for the Internet of Things: the ThingPark platform'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
x-kinRank: "7"
x-alexaRank: "637591"
tags: Generates
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/generates/master/_listings/actility/apis.md
specificationVersion: "0.14"
apis:
- name: ThingPark DX Core API - Access code generation
  x-api-slug: accesscodes-post
  description: Generates a new access code. If it is of type 'userAccessCode', the
    provided userId must reference an user within authorized scopes. This access code
    can then be used to access the targetted application without re-typing credentials
    (ThingPark SSO). In order to do so, the code needs to be appended to the application
    portal URL, i.e. 'portalUrl?userAccessCode=code'.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/generates/master/_listings/actility/accesscodes-post-openapi.md
- name: ThingPark DX Core API - Access code generation
  x-api-slug: accesscodes-post
  description: Generates a new access code. If it is of type 'userAccessCode', the
    provided userId must reference an user within authorized scopes. This access code
    can then be used to access the targetted application without re-typing credentials
    (ThingPark SSO). In order to do so, the code needs to be appended to the application
    portal URL, i.e. 'portalUrl?userAccessCode=code'.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//core/v141/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/generates/master/_listings/actility/accesscodes-post-openapi.md
- name: ThingPark DX Maker API - AppKey generation
  x-api-slug: appkeygens-post
  description: Generate some encrypted VendorKeys with an HSM. Encrypted VendorKeys
    can be decrypted with the private part of provided RSA key. A VendorKey is a concatenation
    of an AppKey (128 bits) and hsmEncryptedAppKey (128 bits).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28250-actility.jpg
  humanURL: https://www.actility.com
  baseURL: https://dx-api.thingpark.com//maker/v011/api
  tags: Technology, SaaS, Enterprise, ISP, Telecommunications, Internet of Things,
    API Provider, Parking, Sensors, Energy, Industrial, Profiles, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/generates/master/_listings/actility/appkeygens-post-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.actility.com/blog/feed/
- type: x-github
  url: https://github.com/actility
- type: x-openapi
  url: https://dx-api.thingpark.com/core/latest/tpdx-core-api-contract.json
- type: x-api-gallery
  url: http://actility.api.gallery.streamdata.io
- type: x-api-stack
  url: http://actility.stack.network
- type: x-blog
  url: https://www.actility.com/blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/actility
- type: x-developer
  url: https://www.actility.com/developer/
- type: x-twitter
  url: https://twitter.com/Actility
- type: x-website
  url: https://www.actility.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---