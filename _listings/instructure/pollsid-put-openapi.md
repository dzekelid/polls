---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Polls API Update a single poll
  description: Update a single poll.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /polls:
    get:
      summary: List polls
      description: List polls.
      operationId: list-polls
      x-api-path-slug: polls-get
      responses:
        200:
          description: OK
      tags:
      - Polls
    post:
      summary: Create a single poll
      description: Create a single poll.
      operationId: create-a-single-poll
      x-api-path-slug: polls-post
      parameters:
      - in: query
        name: polls[][description]
        description: A brief description or instructions for the poll
      - in: query
        name: polls[][question]
        description: The title of the poll
      responses:
        200:
          description: OK
      tags:
      - Polls
  /polls/{id}:
    delete:
      summary: Delete a poll
      description: Delete a poll.
      operationId: delete-a-poll
      x-api-path-slug: pollsid-delete
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Id
    get:
      summary: Get a single poll
      description: Get a single poll.
      operationId: get-a-single-poll
      x-api-path-slug: pollsid-get
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Id
    put:
      summary: Update a single poll
      description: Update a single poll.
      operationId: update-a-single-poll
      x-api-path-slug: pollsid-put
      parameters:
      - in: query
        name: polls[][description]
        description: A brief description or instructions for the poll
      - in: query
        name: polls[][question]
        description: The title of the poll
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Id
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