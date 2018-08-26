---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 1
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
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
---