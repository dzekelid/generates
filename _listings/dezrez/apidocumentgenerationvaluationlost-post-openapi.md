---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Generates a Valuation Lost letter correspondence to the vendor of
    a particular marketing role
  version: 1.0.0
  description: Generates a valuation lost letter correspondence to the vendor of a
    particular marketing role.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/custompack:
    post:
      summary: Generates any correspondence and can allow you to overpost information
        to the correspondence
      description: Generates any correspondence and can allow you to overpost information
        to the correspondence.
      operationId: DocumentGeneration_GeneratePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcustompack-post
      parameters:
      - in: body
        name: generatePackDetails
        description: broad contract that allows for overposting and underposting,
          however you must specify a correspondence Id            you must then follow
          the validation rules for the for that individual correspondence type, each
          route to the controller is named in the same way            as the enumerated
          correspondence type system name, and the mappings for the specific class
          to the GeneratePackJobDataContract are detailed in             the each
          individual simplified contract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Any
      - Correspondence
      - Can
      - Ow
      - You
      - To
      - Overpost
      - Information
      - To
      - Correspondence
  /api/documentgeneration/previewpack:
    post:
      summary: Generates a pack using the first selected group/property of a type
        to get a quick preview of the pack
      description: Generates a pack using the first selected group/property of a type
        to get a quick preview of the pack.
      operationId: DocumentGeneration_PreviewPackByrandomPackDataContract
      x-api-path-slug: apidocumentgenerationpreviewpack-post
      parameters:
      - in: body
        name: randomPackDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Pack
      - Using
      - First
      - Selected
      - Group
      - Property
      - Of
      - Type
      - To
      - Get
      - Quick
      - Preview
      - Of
      - Pack
  /api/documentgeneration/boardordernew:
    post:
      summary: Generates an board ordering New correspondence
      description: Generates an board ordering new correspondence.
      operationId: DocumentGeneration_BoardOrderingNewPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardordernew-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Board
      - Ordering
      - New
      - Correspondence
  /api/documentgeneration/boardorderreplace:
    post:
      summary: Generates an board ordering Replace correspondence
      description: Generates an board ordering replace correspondence.
      operationId: DocumentGeneration_BoardOrderReplacePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardorderreplace-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Board
      - Ordering
      - Replace
      - Correspondence
  /api/documentgeneration/boardordertakedown:
    post:
      summary: Generates an board ordering Takedown correspondence
      description: Generates an board ordering takedown correspondence.
      operationId: DocumentGeneration_BoardOrderTakedownPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardordertakedown-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Board
      - Ordering
      - Takedown
      - Correspondence
  /api/documentgeneration/boardorderupdate:
    post:
      summary: Generates an board ordering Update correspondence
      description: Generates an board ordering update correspondence.
      operationId: DocumentGeneration_BoardOrderUpdatePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardorderupdate-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Board
      - Ordering
      - ""
      - Correspondence
  /api/documentgeneration/confirmvaluation:
    post:
      summary: Generates a correspondence confirming the booking of a valuation appointment.  Uses
        default values where possible.
      description: Generates a correspondence confirming the booking of a valuation
        appointment.  uses default values where possible..
      operationId: DocumentGeneration_GenerateValuationConfirmationLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmvaluation-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Confirming
      - Booking
      - Of
      - Valuation
      - Appointment
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/valuationresult:
    post:
      summary: Generates a correspondence confirming the result of a valuation appointment.  Uses
        default values where possible.
      description: Generates a correspondence confirming the result of a valuation
        appointment.  uses default values where possible..
      operationId: DocumentGeneration_GenerateValuationResultLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvaluationresult-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Confirming
      - Result
      - Of
      - Valuation
      - Appointment
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/instruction:
    post:
      summary: Generates a Instruction letter correspondence to the vendor of a particular
        marketing role
      description: Generates a instruction letter correspondence to the vendor of
        a particular marketing role.
      operationId: DocumentGeneration_GenerateInstructionLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationinstruction-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Instruction
      - Letter
      - Correspondence
      - To
      - Vendor
      - Of
      - Particular
      - Marketing
      - Role
  /api/documentgeneration/tenancyagreementast:
    post:
      summary: Generates Tenancy Agreement correspondence
      description: Generates tenancy agreement correspondence.
      operationId: DocumentGeneration_TenancyAgreementASTBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationtenancyagreementast-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Tenancy
      - Agreement
      - Correspondence
  /api/documentgeneration/tenancyguarantor:
    post:
      summary: Generates Tenancy Guarantor correspondence
      description: Generates tenancy guarantor correspondence.
      operationId: DocumentGeneration_TenancyGuarantorBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationtenancyguarantor-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Tenancy
      - Guarantor
      - Correspondence
  /api/documentgeneration/withdrawninstruction:
    post:
      summary: Generates a Withdrawn Instruction letter correspondence to the vendor
        of a particular marketing role
      description: Generates a withdrawn instruction letter correspondence to the
        vendor of a particular marketing role.
      operationId: DocumentGeneration_GenerateWithdrawnInstructionLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationwithdrawninstruction-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Withdrawn
      - Instruction
      - Letter
      - Correspondence
      - To
      - Vendor
      - Of
      - Particular
      - Marketing
      - Role
  /api/documentgeneration/reschedulevaluation:
    post:
      summary: Generates a Reschedule Valuation letter correspondence
      description: Generates a reschedule valuation letter correspondence.
      operationId: DocumentGeneration_RescheduleValuationLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationreschedulevaluation-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Reschedule
      - Valuation
      - Letter
      - Correspondence
  /api/documentgeneration/valuationlost:
    post:
      summary: Generates a Valuation Lost letter correspondence to the vendor of a
        particular marketing role
      description: Generates a valuation lost letter correspondence to the vendor
        of a particular marketing role.
      operationId: DocumentGeneration_GenerateValuationLostLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvaluationlost-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Valuation
      - Lost
      - Letter
      - Correspondence
      - To
      - Vendor
      - Of
      - Particular
      - Marketing
      - Role
  /api/documentgeneration/rescheduleepcappointment:
    post:
      summary: Generates a EPC Appointment letter correspondence
      description: Generates a epc appointment letter correspondence.
      operationId: DocumentGeneration_RescheduleEpcAppointmentLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationrescheduleepcappointment-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - EPC
      - Appointment
      - Letter
      - Correspondence
  /api/documentgeneration/reschedulemeeting:
    post:
      summary: Generates a meeting letter correspondence
      description: Generates a meeting letter correspondence.
      operationId: DocumentGeneration_ReschedulMeetingLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationreschedulemeeting-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Meeting
      - Letter
      - Correspondence
  /api/documentgeneration/cancelvaluation:
    post:
      summary: Generates a cancel a valuation letter correspondence
      description: Generates a cancel a valuation letter correspondence.
      operationId: DocumentGeneration_CancelValuationLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancelvaluation-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Cancel
      - Valuation
      - Letter
      - Correspondence
  /api/documentgeneration/cancelepcappointment:
    post:
      summary: Generates a cancel an epc appointment letter correspondence
      description: Generates a cancel an epc appointment letter correspondence.
      operationId: DocumentGeneration_CancelEpcAppointmentLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancelepcappointment-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Cancel
      - Epc
      - Appointment
      - Letter
      - Correspondence
  /api/documentgeneration/confirmepcappointment:
    post:
      summary: Generates a confirm an epc appointment letter correspondence
      description: Generates a confirm an epc appointment letter correspondence.
      operationId: DocumentGeneration_ConfirmEpcAppointmentLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmepcappointment-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Confirm
      - Epc
      - Appointment
      - Letter
      - Correspondence
  /api/documentgeneration/cancelmeeting:
    post:
      summary: Generates a cancel a meeting letter correspondence
      description: Generates a cancel a meeting letter correspondence.
      operationId: DocumentGeneration_CancelMeetingLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancelmeeting-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Cancel
      - Meeting
      - Letter
      - Correspondence
  /api/documentgeneration/confirmmeeting:
    post:
      summary: Generates a confirm a meeting letter correspondence
      description: Generates a confirm a meeting letter correspondence.
      operationId: DocumentGeneration_ConfirmMeetingLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmmeeting-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Confirm
      - Meeting
      - Letter
      - Correspondence
  /api/documentgeneration/confirmgeneralappointment:
    post:
      summary: Generates a confirm general appointment letter correspondence
      description: Generates a confirm general appointment letter correspondence.
      operationId: DocumentGeneration_ConfirmGeneralAppointmentLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmgeneralappointment-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Confirm
      - General
      - Appointment
      - Letter
      - Correspondence
  /api/documentgeneration/cancelgeneralappointment:
    post:
      summary: Generates a cancel general appointment letter correspondence
      description: Generates a cancel general appointment letter correspondence.
      operationId: DocumentGeneration_CancelGeneralAppointmentLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancelgeneralappointment-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Cancel
      - General
      - Appointment
      - Letter
      - Correspondence
  /api/documentgeneration/reschedulegeneralappointment:
    post:
      summary: Generates a reschedule general appointment letter correspondence
      description: Generates a reschedule general appointment letter correspondence.
      operationId: DocumentGeneration_RescheduleGeneralAppointmentLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationreschedulegeneralappointment-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Reschedule
      - General
      - Appointment
      - Letter
      - Correspondence
  /api/documentgeneration/offer:
    post:
      summary: Generates a correspondence notifying the vendor of an offer.  Uses
        default values where possible.
      description: Generates a correspondence notifying the vendor of an offer.  uses
        default values where possible..
      operationId: DocumentGeneration_OfferLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationoffer-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Notifying
      - Vendor
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offeraccepted:
    post:
      summary: Generates a correspondence any parties of the acceptance of an offer.  Uses
        default values where possible.
      description: Generates a correspondence any parties of the acceptance of an
        offer.  uses default values where possible..
      operationId: DocumentGeneration_OfferAcceptedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferaccepted-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Any
      - Parties
      - Of
      - Acceptance
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offerrejected:
    post:
      summary: Generates a correspondence any parties of the rejection of an offer.  Uses
        default values where possible.
      description: Generates a correspondence any parties of the rejection of an offer.  uses
        default values where possible..
      operationId: DocumentGeneration_OfferRejectedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferrejected-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Any
      - Parties
      - Of
      - Rejection
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offerwithdrawn:
    post:
      summary: Generates a correspondence to notify any parties of the withdrawl of
        an offer.  Uses default values where possible.
      description: Generates a correspondence to notify any parties of the withdrawl
        of an offer.  uses default values where possible..
      operationId: DocumentGeneration_OfferwithdrawnLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferwithdrawn-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Withdrawl
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/completed:
    post:
      summary: Generates a correspondence to notify any parties of completion.  Uses
        default values where possible.
      description: Generates a correspondence to notify any parties of completion.  uses
        default values where possible..
      operationId: DocumentGeneration_CompletedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcompleted-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Completion
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/exchanged:
    post:
      summary: Generates a correspondence to notify any parties of exchanged.  Uses
        default values where possible.
      description: Generates a correspondence to notify any parties of exchanged.  uses
        default values where possible..
      operationId: DocumentGeneration_ExchangedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationexchanged-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Exchanged
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/openhouse:
    post:
      summary: Generates an open house correspondence
      description: Generates an open house correspondence.
      operationId: DocumentGeneration_OpenHouseLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationopenhouse-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Open
      - House
      - Correspondence
  /api/documentgeneration/confirmationofviewing:
    post:
      summary: Generates a correspondence to notify all parties of a scheduled viewing.  Uses
        default values where possible.
      description: Generates a correspondence to notify all parties of a scheduled
        viewing.  uses default values where possible..
      operationId: DocumentGeneration_ConfirmationOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmationofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - ""
      - Parties
      - Of
      - Scheduled
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/cancellationofviewing:
    post:
      summary: Generates a correspondence to notify parties of a cancellation of a
        viewing.  Uses default values where possible.
      description: Generates a correspondence to notify parties of a cancellation
        of a viewing.  uses default values where possible..
      operationId: DocumentGeneration_CancellationOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancellationofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Parties
      - Of
      - Cancellation
      - Of
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/reschedulingofviewing:
    post:
      summary: Generates a correspondence to notify parties involved of a rescheduling
        of a viewing.  Uses default values where possible.
      description: Generates a correspondence to notify parties involved of a rescheduling
        of a viewing.  uses default values where possible..
      operationId: DocumentGeneration_ReschedulingOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationreschedulingofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Parties
      - Involved
      - Of
      - Rescheduling
      - Of
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/singlepropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them all
        the same property role
      description: Generates a correspondence to multiple applicants, sending them
        all the same property role.
      operationId: DocumentGeneration_SendPropertyToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsinglepropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - ""
      - Same
      - Property
      - Role
  /api/documentgeneration/singlelettingspropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them all
        the same letting property role
      description: Generates a correspondence to multiple applicants, sending them
        all the same letting property role.
      operationId: DocumentGeneration_SendLettingsPropertyToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsinglelettingspropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - ""
      - Same
      - Letting
      - Property
      - Role
  /api/documentgeneration/printablepropertylist:
    post:
      summary: Generates a printable property list, it is targetless so there is no
        reference to applicants or owners
      description: Generates a printable property list, it is targetless so there
        is no reference to applicants or owners.
      operationId: DocumentGeneration_PrintablePropertyListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationprintablepropertylist-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Printable
      - Property
      - List
      - ""
      - It
      - Is
      - Targetless
      - So
      - There
      - Is
      - "No"
      - Reference
      - To
      - Applicants
      - Owners
  /api/documentgeneration/selectedpropertiesmatch:
    post:
      summary: Generates a correspondence to a single applicant, sending them user
        selected property roles
      description: Generates a correspondence to a single applicant, sending them
        user selected property roles.
      operationId: DocumentGeneration_SendSelectedPropertiesToApplicantBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationselectedpropertiesmatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Single
      - Applicant
      - ""
      - Sending
      - Them
      - User
      - Selected
      - Property
      - Roles
  /api/documentgeneration/selectedlettingspropertiesmatch:
    post:
      summary: Generates a correspondence to a single letting applicant, sending them
        user selected property roles
      description: Generates a correspondence to a single letting applicant, sending
        them user selected property roles.
      operationId: DocumentGeneration_SendSelectedLettingsPropertiesToApplicantBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationselectedlettingspropertiesmatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Single
      - Letting
      - Applicant
      - ""
      - Sending
      - Them
      - User
      - Selected
      - Property
      - Roles
  /api/documentgeneration/multipropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them a filtered
        set of the matching property roles
      description: Generates a correspondence to multiple applicants, sending them
        a filtered set of the matching property roles.
      operationId: DocumentGeneration_SendAutoMatchedPropertiesToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationmultipropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - Filtered
      - Set
      - Of
      - Matching
      - Property
      - Roles
  /api/documentgeneration/multilettingspropertymatch:
    post:
      summary: Generates a correspondence to multiple letting applicants, sending
        them a filtered set of the matching letting property roles
      description: Generates a correspondence to multiple letting applicants, sending
        them a filtered set of the matching letting property roles.
      operationId: DocumentGeneration_SendAutoMatchedLettingsPropertiesToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationmultilettingspropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Letting
      - Applicants
      - ""
      - Sending
      - Them
      - Filtered
      - Set
      - Of
      - Matching
      - Letting
      - Property
      - Roles
  /api/documentgeneration/vendorreport:
    post:
      summary: Generates a correspondence to a single group, sending them a single
        report for multiple properties
      description: Generates a correspondence to a single group, sending them a single
        report for multiple properties.
      operationId: DocumentGeneration_SendVendorReportBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvendorreport-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Single
      - Group
      - ""
      - Sending
      - Them
      - Single
      - Reportmultiple
      - Properties
  /api/documentgeneration/salesapplicantwelcomepack:
    post:
      summary: Generates a correspondence to a an sales applicant
      description: Generates a correspondence to a an sales applicant.
      operationId: DocumentGeneration_SalesApplicantWelcomePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsalesapplicantwelcomepack-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Sales
      - Applicant
  /api/documentgeneration/lettingsapplicantwelcomepack:
    post:
      summary: Generates a correspondence to a an lettings applicant
      description: Generates a correspondence to a an lettings applicant.
      operationId: DocumentGeneration_LettingsApplicantWelcomePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationlettingsapplicantwelcomepack-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Lettings
      - Applicant
  /api/documentgeneration/vendorwelcomepack:
    post:
      summary: Generates a correspondence to a an lettings applicant
      description: Generates a correspondence to a an lettings applicant.
      operationId: DocumentGeneration_VendorWelcomePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvendorwelcomepack-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Lettings
      - Applicant
  /api/documentgeneration/bulkgrouplistcommunication:
    post:
      summary: Generates a bulk communication pack out to multiple clients in a list.
      description: Generates a bulk communication pack out to multiple clients in
        a list..
      operationId: DocumentGeneration_BulkGroupListCommunicationBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationbulkgrouplistcommunication-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Bulk
      - Communication
      - Pack
      - Out
      - To
      - Multiple
      - Clients
      - In
      - List
  /api/documentgeneration/bulkinterestrolecommunication:
    post:
      summary: Generates a bulk communication pack out to multiple clients with interest
        roles.
      description: Generates a bulk communication pack out to multiple clients with
        interest roles..
      operationId: DocumentGeneration_BulkInterestRoleCommunicationBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationbulkinterestrolecommunication-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Bulk
      - Communication
      - Pack
      - Out
      - To
      - Multiple
      - Clients
      - Interest
      - Roles
  /api/documentgeneration/bulkpropertyownercommunication:
    post:
      summary: "Generates a bulk communication pack out to multiple vendors of properties.\r\nThis
        will ignore the target type set, as the document could only ever find the
        vendor as the contact item, so it always defaults\r\nto a target type of vendor/owner"
      description: "Generates a bulk communication pack out to multiple vendors of
        properties.\r\nthis will ignore the target type set, as the document could
        only ever find the vendor as the contact item, so it always defaults\r\nto
        a target type of vendor/owner."
      operationId: DocumentGeneration_BulkPropertyVendorCommunicationBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationbulkpropertyownercommunication-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Bulk
      - Communication
      - Pack
      - Out
      - To
      - Multiple
      - Vendors
      - Of
      - Properties
      - This
      - Will
      - Ignore
      - Target
      - Type
      - Set
      - ""
      - As
      - Document
      - Could
      - Only
      - Ever
      - Find
      - Vendor
      - As
      - Contact
      - Item
      - ""
      - So
      - It
      - Always
      - "Defaults\r\nTo"
      - Target
      - Type
      - Of
      - Vendor
      - Owner
  /api/list/property/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/lettingproperty/csv:
    post:
      summary: Generates a csv file from selected letting property list items
      description: Generates a csv file from selected letting property list items.
      operationId: List_GenerateLettingPropertyCsvBycommandDataContract
      x-api-path-slug: apilistlettingpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Letting
      - Property
      - List
      - Items
  /api/list/propertypipeline/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePipelinePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertypipelinecsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/events/csv:
    post:
      summary: Generates a csv file from selected event list items
      description: Generates a csv file from selected event list items.
      operationId: List_GenerateEventCsvBycommandDataContract
      x-api-path-slug: apilisteventscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Event
      - List
      - Items
  /api/list/groups/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateGroupCsvBycommandDataContract
      x-api-path-slug: apilistgroupscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/groupinterests/csv:
    post:
      summary: Generates a csv file from selected group interest list items
      description: Generates a csv file from selected group interest list items.
      operationId: List_GenerateGroupInterestCsvBycommandDataContract
      x-api-path-slug: apilistgroupinterestscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - Interest
      - List
      - Items
  /api/list/activesearches/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateActiveSearchCsvBycommandDataContract
      x-api-path-slug: apilistactivesearchescsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/groupmatches/csv:
    post:
      summary: Generates a csv file from group matches by property role id
      description: Generates a csv file from group matches by property role id.
      operationId: List_GenerateGroupMatchesCsvBycommandDataContract
      x-api-path-slug: apilistgroupmatchescsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Group
      - Matches
      - By
      - Property
      - Role
      - Id
  /api/list/propertyfinancial/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateFinancialPropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertyfinancialcsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/propertynewbusiness/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GenerateNewBusinessPropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertynewbusinesscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/cache/Key:
    get:
      summary: Generate a guid for use as a key
      description: Generate a guid for use as a key.
      operationId: Cache_GenerateKey
      x-api-path-slug: apicachekey-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Guiduse
      - As
      - Key
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