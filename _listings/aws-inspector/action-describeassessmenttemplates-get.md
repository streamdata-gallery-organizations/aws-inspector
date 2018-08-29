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
  /?Action=DescribeAssessmentTemplates:
    get:
      summary: ' Describe Assessment Templates '
      description: |-
        Describes the assessment templates that are specified by the ARNs of the assessment
                 templates
      operationId: describeAssessmentTemplates
      parameters:
      - in: query
        name: assessmentTemplateArns
        description: 'Type: array of Strings'
        type: string
      responses:
        200:
          description: OK
      tags:
      - assessment templates
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