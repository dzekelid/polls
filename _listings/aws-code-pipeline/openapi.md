---
swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 1
info:
  title: AWS Code Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PollForJobs:
    get:
      summary: Poll For Jobs
      description: Returns information about any jobs for AWS CodePipeline to act
        upon.
      operationId: pollForJobs
      x-api-path-slug: actionpollforjobs-get
      parameters:
      - in: query
        name: actionTypeId
        description: Represents information about an action type
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: maxBatchSize
        description: The maximum number of jobs to return in a poll for jobs call
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: NextToken
        description: The token to use to retrieve the next page of results
        type: string
      - in: query
        name: PublicIp.N
        description: One or more Elastic IP addresses
        type: string
      - in: query
        name: queryParam
        description: A map of property names and values
        type: string
      responses:
        200:
          description: OK
      tags:
      - PollJobs
  /?Action=PollForThirdPartyJobs:
    get:
      summary: Poll For Third Party Jobs
      description: Determines whether there are any third party jobs for a job worker
        to act on.
      operationId: pollForThirdPartyJobs
      x-api-path-slug: actionpollforthirdpartyjobs-get
      parameters:
      - in: query
        name: actionTypeId
        description: Represents information about an action type
        type: string
      - in: query
        name: AssociationId
        description: '[EC2-VPC] The association ID'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: maxBatchSize
        description: The maximum number of jobs to return in a poll for jobs call
        type: string
      - in: query
        name: PublicIp
        description: '[EC2-Classic] The Elastic IP address'
        type: string
      responses:
        200:
          description: OK
      tags:
      - PollThird
      - Party
      - Jobs
---