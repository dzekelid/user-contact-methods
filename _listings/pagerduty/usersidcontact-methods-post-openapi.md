---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 0
info:
  title: PagerDuty Create a user contact method
  version: 1.0.0
  description: Create a new contact method.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{id}/contact_methods:
    get:
      summary: List a user's contact methods
      description: List contact methods of your PagerDuty user.
      operationId: list-contact-methods-of-your-pagerduty-user
      x-api-path-slug: usersidcontact-methods-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - User Contact Methods
    post:
      summary: Create a user contact method
      description: Create a new contact method.
      operationId: create-a-new-contact-method
      x-api-path-slug: usersidcontact-methods-post
      parameters:
      - in: body
        name: contact_method
        description: The contact method to be created
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - User Contact Methods
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