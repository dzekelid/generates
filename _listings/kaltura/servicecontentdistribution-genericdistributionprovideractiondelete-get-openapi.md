---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Contentdistribution Genericdistributionprover Action
    Delete
  description: Delete Generic Distribution Provider by id
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/contentdistribution_genericdistributionprovider/action/add:
    get:
      summary: Get Service Contentdistribution Genericdistributionprover Action Add
      description: Add new Generic Distribution Provider
      operationId: genericDistributionProvider.add
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionadd-get
      parameters:
      - in: query
        name: genericDistributionProvider[availabilityUpdateEnabled]
      - in: query
        name: genericDistributionProvider[deleteInsteadUpdate]
      - in: query
        name: genericDistributionProvider[editableFields]
      - in: query
        name: genericDistributionProvider[intervalBeforeSunrise]
      - in: query
        name: genericDistributionProvider[intervalBeforeSunset]
      - in: query
        name: genericDistributionProvider[isDefault]
      - in: query
        name: genericDistributionProvider[mandatoryFields]
      - in: query
        name: genericDistributionProvider[name]
      - in: query
        name: genericDistributionProvider[optionalFlavorParamsIds]
      - in: query
        name: genericDistributionProvider[optionalThumbDimensions]
      - in: query
        name: genericDistributionProvider[requiredFlavorParamsIds]
      - in: query
        name: genericDistributionProvider[requiredThumbDimensions]
      - in: query
        name: genericDistributionProvider[scheduleUpdateEnabled]
      - in: query
        name: genericDistributionProvider[updateRequiredEntryFields]
      - in: query
        name: genericDistributionProvider[updateRequiredMetadataXPaths]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovider
      - Action
      - Add
  /service/contentdistribution_genericdistributionprovider/action/delete:
    get:
      summary: Get Service Contentdistribution Genericdistributionprover Action Delete
      description: Delete Generic Distribution Provider by id
      operationId: genericDistributionProvider.delete
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovider
      - Action
      - Delete
  /service/contentdistribution_genericdistributionprovider/action/get:
    get:
      summary: Get Service Contentdistribution Genericdistributionprover Action Get
      description: Get Generic Distribution Provider by id
      operationId: genericDistributionProvider.get
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovider
      - Action
      - Get
  /service/contentdistribution_genericdistributionprovider/action/list:
    get:
      summary: Get Service Contentdistribution Genericdistributionprover Action List
      description: List all distribution providers
      operationId: genericDistributionProvider.list
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[isDefaultEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[isDefaultIn]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaGenericDistributionProviderStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[typeEqual]
        description: 'Enum Type: `KalturaDistributionProviderType`'
      - in: query
        name: filter[typeIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovider
      - Action
      - List
  /service/contentdistribution_genericdistributionprovider/action/update:
    get:
      summary: Get Service Contentdistribution Genericdistributionprover Action Update
      description: Update Generic Distribution Provider by id
      operationId: genericDistributionProvider.update
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionupdate-get
      parameters:
      - in: query
        name: genericDistributionProvider[availabilityUpdateEnabled]
      - in: query
        name: genericDistributionProvider[deleteInsteadUpdate]
      - in: query
        name: genericDistributionProvider[editableFields]
      - in: query
        name: genericDistributionProvider[intervalBeforeSunrise]
      - in: query
        name: genericDistributionProvider[intervalBeforeSunset]
      - in: query
        name: genericDistributionProvider[isDefault]
      - in: query
        name: genericDistributionProvider[mandatoryFields]
      - in: query
        name: genericDistributionProvider[name]
      - in: query
        name: genericDistributionProvider[optionalFlavorParamsIds]
      - in: query
        name: genericDistributionProvider[optionalThumbDimensions]
      - in: query
        name: genericDistributionProvider[requiredFlavorParamsIds]
      - in: query
        name: genericDistributionProvider[requiredThumbDimensions]
      - in: query
        name: genericDistributionProvider[scheduleUpdateEnabled]
      - in: query
        name: genericDistributionProvider[updateRequiredEntryFields]
      - in: query
        name: genericDistributionProvider[updateRequiredMetadataXPaths]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovider
      - Action
      - Update
  /service/contentdistribution_genericdistributionprovideraction/action/add:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Add
      description: Add new Generic Distribution Provider Action
      operationId: genericDistributionProviderAction.add
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionadd-get
      parameters:
      - in: query
        name: genericDistributionProviderAction[action]
        description: '`insertOnly`Enum Type: `KalturaDistributionAction`'
      - in: query
        name: genericDistributionProviderAction[editableFields]
      - in: query
        name: genericDistributionProviderAction[genericDistributionProviderId]
        description: '`insertOnly`'
      - in: query
        name: genericDistributionProviderAction[mandatoryFields]
      - in: query
        name: genericDistributionProviderAction[protocol]
        description: 'Enum Type: `KalturaDistributionProtocol`'
      - in: query
        name: genericDistributionProviderAction[remotePassword]
      - in: query
        name: genericDistributionProviderAction[remotePath]
      - in: query
        name: genericDistributionProviderAction[remoteUsername]
      - in: query
        name: genericDistributionProviderAction[resultsParser]
        description: 'Enum Type: `KalturaGenericDistributionProviderParser`'
      - in: query
        name: genericDistributionProviderAction[serverAddress]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - Add
  /service/contentdistribution_genericdistributionprovideraction/action/addMrssTransform:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Addmrsstransform
      description: Add MRSS transform file to generic distribution provider action
      operationId: genericDistributionProviderAction.addMrssTransform
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionaddmrsstransform-get
      parameters:
      - in: query
        name: id
        description: the id of the generic distribution provider action
      - in: query
        name: No Name
      - in: query
        name: xslData
        description: XSL MRSS transformation data
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - AddMrssTransform
  /service/contentdistribution_genericdistributionprovideraction/action/addMrssTransformFromFile:
    post:
      summary: Post Service Contentdistribution Genericdistributionproveraction Action
        Addmrsstransformfromfile
      description: Add MRSS transform file to generic distribution provider action
      operationId: genericDistributionProviderAction.addMrssTransformFromFile
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionaddmrsstransformfromfile-post
      parameters:
      - in: query
        name: id
        description: the id of the generic distribution provider action
      - in: query
        name: No Name
      - in: formData
        name: xslFile
        description: XSL MRSS transformation file
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - AddMrssTransformFromFile
  /service/contentdistribution_genericdistributionprovideraction/action/addMrssValidate:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Addmrssvalate
      description: Add MRSS validate file to generic distribution provider action
      operationId: genericDistributionProviderAction.addMrssValidate
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionaddmrssvalidate-get
      parameters:
      - in: query
        name: id
        description: the id of the generic distribution provider action
      - in: query
        name: No Name
      - in: query
        name: xsdData
        description: XSD MRSS validatation data
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - AddMrssValidate
  /service/contentdistribution_genericdistributionprovideraction/action/addMrssValidateFromFile:
    post:
      summary: Post Service Contentdistribution Genericdistributionproveraction Action
        Addmrssvalatefromfile
      description: Add MRSS validate file to generic distribution provider action
      operationId: genericDistributionProviderAction.addMrssValidateFromFile
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionaddmrssvalidatefromfile-post
      parameters:
      - in: query
        name: id
        description: the id of the generic distribution provider action
      - in: query
        name: No Name
      - in: formData
        name: xsdFile
        description: XSD MRSS validatation file
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - AddMrssValidateFromFile
  /service/contentdistribution_genericdistributionprovideraction/action/addResultsTransform:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Addresultstransform
      description: Add results transform file to generic distribution provider action
      operationId: genericDistributionProviderAction.addResultsTransform
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionaddresultstransform-get
      parameters:
      - in: query
        name: id
        description: the id of the generic distribution provider action
      - in: query
        name: No Name
      - in: query
        name: transformData
        description: transformation data xsl, xPath or regex
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - AddResultsTransform
  /service/contentdistribution_genericdistributionprovideraction/action/addResultsTransformFromFile:
    post:
      summary: Post Service Contentdistribution Genericdistributionproveraction Action
        Addresultstransformfromfile
      description: Add MRSS transform file to generic distribution provider action
      operationId: genericDistributionProviderAction.addResultsTransformFromFile
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionaddresultstransformfromfile-post
      parameters:
      - in: query
        name: id
        description: the id of the generic distribution provider action
      - in: query
        name: No Name
      - in: formData
        name: transformFile
        description: transformation file xsl, xPath or regex
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - AddResultsTransformFromFile
  /service/contentdistribution_genericdistributionprovideraction/action/delete:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Delete
      description: Delete Generic Distribution Provider Action by id
      operationId: genericDistributionProviderAction.delete
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - Delete
  /service/contentdistribution_genericdistributionprovideraction/action/deleteByProviderId:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Deletebyproverid
      description: Delete Generic Distribution Provider Action by provider id
      operationId: genericDistributionProviderAction.deleteByProviderId
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactiondeletebyproviderid-get
      parameters:
      - in: query
        name: actionType
        description: 'Enum Type: `KalturaDistributionAction`'
      - in: query
        name: genericDistributionProviderId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - DeleteByProviderId
  /service/contentdistribution_genericdistributionprovideraction/action/get:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Get
      description: Get Generic Distribution Provider Action by id
      operationId: genericDistributionProviderAction.get
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - Get
  /service/contentdistribution_genericdistributionprovideraction/action/getByProviderId:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Getbyproverid
      description: Get Generic Distribution Provider Action by provider id
      operationId: genericDistributionProviderAction.getByProviderId
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactiongetbyproviderid-get
      parameters:
      - in: query
        name: actionType
        description: 'Enum Type: `KalturaDistributionAction`'
      - in: query
        name: genericDistributionProviderId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - GetByProviderId
  /service/contentdistribution_genericdistributionprovideraction/action/list:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        List
      description: List all distribution providers
      operationId: genericDistributionProviderAction.list
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionlist-get
      parameters:
      - in: query
        name: filter[actionEqual]
        description: 'Enum Type: `KalturaDistributionAction`'
      - in: query
        name: filter[actionIn]
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[genericDistributionProviderIdEqual]
      - in: query
        name: filter[genericDistributionProviderIdIn]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - List
  /service/contentdistribution_genericdistributionprovideraction/action/update:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Update
      description: Update Generic Distribution Provider Action by id
      operationId: genericDistributionProviderAction.update
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionupdate-get
      parameters:
      - in: query
        name: genericDistributionProviderAction[action]
        description: '`insertOnly`Enum Type: `KalturaDistributionAction`'
      - in: query
        name: genericDistributionProviderAction[editableFields]
      - in: query
        name: genericDistributionProviderAction[genericDistributionProviderId]
        description: '`insertOnly`'
      - in: query
        name: genericDistributionProviderAction[mandatoryFields]
      - in: query
        name: genericDistributionProviderAction[protocol]
        description: 'Enum Type: `KalturaDistributionProtocol`'
      - in: query
        name: genericDistributionProviderAction[remotePassword]
      - in: query
        name: genericDistributionProviderAction[remotePath]
      - in: query
        name: genericDistributionProviderAction[remoteUsername]
      - in: query
        name: genericDistributionProviderAction[resultsParser]
        description: 'Enum Type: `KalturaGenericDistributionProviderParser`'
      - in: query
        name: genericDistributionProviderAction[serverAddress]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - Update
  /service/contentdistribution_genericdistributionprovideraction/action/updateByProviderId:
    get:
      summary: Get Service Contentdistribution Genericdistributionproveraction Action
        Updatebyproverid
      description: Update Generic Distribution Provider Action by provider id
      operationId: genericDistributionProviderAction.updateByProviderId
      x-api-path-slug: servicecontentdistribution-genericdistributionprovideractionactionupdatebyproviderid-get
      parameters:
      - in: query
        name: actionType
        description: 'Enum Type: `KalturaDistributionAction`'
      - in: query
        name: genericDistributionProviderAction[action]
        description: '`insertOnly`Enum Type: `KalturaDistributionAction`'
      - in: query
        name: genericDistributionProviderAction[editableFields]
      - in: query
        name: genericDistributionProviderAction[genericDistributionProviderId]
        description: '`insertOnly`'
      - in: query
        name: genericDistributionProviderAction[mandatoryFields]
      - in: query
        name: genericDistributionProviderAction[protocol]
        description: 'Enum Type: `KalturaDistributionProtocol`'
      - in: query
        name: genericDistributionProviderAction[remotePassword]
      - in: query
        name: genericDistributionProviderAction[remotePath]
      - in: query
        name: genericDistributionProviderAction[remoteUsername]
      - in: query
        name: genericDistributionProviderAction[resultsParser]
        description: 'Enum Type: `KalturaGenericDistributionProviderParser`'
      - in: query
        name: genericDistributionProviderAction[serverAddress]
      - in: query
        name: genericDistributionProviderId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Genericdistributionprovideraction
      - Action
      - UpdateByProviderId
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