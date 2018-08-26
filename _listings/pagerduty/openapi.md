---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 1
info:
  title: PagerDuty
  version: 1.0.0
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
  /users/{id}/contact_methods/{contact_method_id}:
    get:
      summary: Get a user's contact method
      description: Get details about a user's contact method.
      operationId: get-details-about-a-users-contact-method
      x-api-path-slug: usersidcontact-methodscontact-method-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - User Contact Methods
    delete:
      summary: Delete a user's contact method
      description: Delete users  contact methods contact method
      operationId: remove-a-users-contact-method
      x-api-path-slug: usersidcontact-methodscontact-method-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - User Contact Methods
    put:
      summary: Update a user's contact method
      description: Put users  contact methods contact method
      operationId: update-a-users-contact-method
      x-api-path-slug: usersidcontact-methodscontact-method-id-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: user
        description: The users contact method to be updated
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User Contact Methods
---