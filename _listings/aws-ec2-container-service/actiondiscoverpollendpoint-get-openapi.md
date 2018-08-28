---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 0
info:
  title: Amazon EC2 Container Service API Discover Poll Endpoint
  version: 1.0.0
  description: This action is only used by the Amazon EC2 Container Service agent,
    and it is not intended for use outside of the agent.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DiscoverPollEndpoint:
    get:
      summary: Discover Poll Endpoint
      description: This action is only used by the Amazon EC2 Container Service agent,
        and it is not intended for use outside of the agent.
      operationId: discoverPollEndpoint
      x-api-path-slug: actiondiscoverpollendpoint-get
      responses:
        200:
          description: OK
      tags:
      - Poll Endpoints
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