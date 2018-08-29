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
  /?Action=RemoveAttributesFromFindings:
    get:
      summary: ' Remove Attributes From Findings '
      description: |-
        Removes entire attributes (key and value pairs) from the findings that are specified
                 by the ARNs of the findings where an attribute with the specified key exists
      operationId: removeAttributesFromFindings
      parameters:
      - in: query
        name: attributeKeys
        description: The array of attribute keys that you want to remove from specified         findings
        type: string
      - in: query
        name: findingArns
        description: The ARNs that specify the findings that you want to remove attributes
          from
        type: string
      responses:
        200:
          description: OK
      tags:
      - attributes from findings
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