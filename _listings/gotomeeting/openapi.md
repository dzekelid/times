swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 1
info:
  title: SCIM
  description: the-scim-api-lets-you-manage-users-in-your-organization--you-can-then-automate-the-provisioning-of-product-licenses-for-these-users-and-they-can-use-your-companys-single-signon-solution-through-an-identity-provider-
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: N/A
host: api.citrixonline.com
basePath: /identity/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizers/{organizerKey}/trainings/{trainingKey}/times:
    put:
      summary: Update Training Times
      description: A request to update a scheduled training's start and end times.
        If the request contains 'notifyTrainers = true' and 'notifyRegistrants = true',
        both organizers and registrants are notified. The response provides the number
        of notified trainers and registrants.
      operationId: updateTrainingTimes
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeytimes-put
      parameters:
      - in: body
        name: body
        description: The new start and end times for the scheduled training
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Trainings
      - TrainingKey
      - Times