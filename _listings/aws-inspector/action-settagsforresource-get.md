---
swagger: "2.0"
info:
  title: AWS Inspector API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetTagsForResource:
    get:
      summary: ' Set Tags For Resource '
      description: |-
        Sets tags (key and value pairs) to the assessment template that is specified by the
                 ARN of the assessment template
      operationId: setTagsForResource
      parameters:
      - in: query
        name: resourceArn
        description: The ARN of the assessment template that you want to set tags
          to
        type: string
      - in: query
        name: tags
        description: A collection of key and value pairs that you want to set to the
          assessment         template
        type: string
      responses:
        200:
          description: OK
      tags:
      - tags for resources
definitions: []
x-collection-name: AWS Inspector
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