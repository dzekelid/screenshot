---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Get Console Screenshot
  version: 1.0.0
  description: Retrieve a JPG-format screenshot of a running instance to help with
    troubleshooting.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetConsoleScreenshot:
    get:
      summary: Get Console Screenshot
      description: Retrieve a JPG-format screenshot of a running instance to help
        with troubleshooting.
      operationId: getconsolescreenshot
      x-api-path-slug: actiongetconsolescreenshot-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the Windows instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Console Screenshot
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