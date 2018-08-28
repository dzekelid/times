swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
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
      description: Update training times.
      operationId: OrganizersTrainingsTimesByOrganizerKeyAndTrainingKeyPut
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeytimes-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Training
      - Times
  /{organizerKey}/webinars/{webinarKey}/meetingtimes:
    get:
      summary: Get webinar meeting times
      description: Get webinar meeting times.
      operationId: WebinarsMeetingtimesByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeymeetingtimes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Webinar
      - Meeting
      - Times