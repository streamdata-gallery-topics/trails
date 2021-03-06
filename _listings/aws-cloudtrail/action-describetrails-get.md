---
swagger: "2.0"
info:
  title: AWS CloudTrail API Describe Trails
  version: 1.0.0
  description: Retrieves settings for the trail associated with the current region
    for your account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeTrails:
    get:
      summary: Describe Trails
      description: Retrieves settings for the trail associated with the current region
        for your account
      operationId: DescribeTrails
      parameters:
      - in: query
        name: includeShadowTrails
        description: Specifies whether to include shadow trails in the response
        type: string
      - in: query
        name: trailNameList
        description: Specifies a list of trail names, trail ARNs, or both, of the
          trails to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - trails
definitions: []
x-collection-name: AWS CloudTrail
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