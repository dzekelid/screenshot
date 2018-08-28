swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
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