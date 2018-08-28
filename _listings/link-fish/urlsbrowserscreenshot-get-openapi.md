---
swagger: "2.0"
x-collection-name: link.fish
x-complete: 0
info:
  title: link.fish Generate screenshot (browser)
  description: Visits the URL with full browser and creates a screenshot. This request
    costs 5 credits.
  termsOfService: https://link.fish/terms-of-service/
  contact:
    name: link.fish
    url: https://link.fish/api
    email: api@link.fish
  version: "2017-12-01"
host: api.link.fish
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Urls/browser-screenshot:
    get:
      summary: Generate screenshot (browser)
      description: Visits the URL with full browser and creates a screenshot. This
        request costs 5 credits.
      operationId: Urls.browser_screenshot.get
      x-api-path-slug: urlsbrowserscreenshot-get
      parameters:
      - in: query
        name: file_format
        description: The file format of the screenshot
      - in: query
        name: type
        description: What kind of screenshot should be returned
      - in: query
        name: url
        description: The URL of the website to create screenshot of
      - in: query
        name: width
        description: The widh of the screenshot in pixel
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Browser
      - Screenshot
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