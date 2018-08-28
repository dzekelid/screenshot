---
name: Browshot
x-slug: browshot
description: Browshot is a service to take screenshot of web pages. Use any of our
  mobile and desktop browsers. We provide a powerful API and libraries.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
x-kinRank: "7"
x-alexaRank: "1714303"
tags: Screenshot
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/apis.md
specificationVersion: "0.14"
apis:
- name: Browshot - Request a screenshot
  x-api-slug: screenshotcreate-get
  description: |-
    Screenshots requests to private and shared instances require a positive balance.

    *IMPORTANT*: Remember that you can only do 100 free screenshots per month. To used a premium instance, use instance_id=65 for example.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotcreate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotcreate-get-openapi.md
- name: Browshot - Delete screenshot data
  x-api-slug: screenshotdelete-get
  description: You can delete details of your screenshots to remove any confidential
    information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotdelete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotdelete-get-openapi.md
- name: Browshot - Host thumbnails on your own S3 account or on Browshot.
  x-api-slug: screenshothost-get
  description: You can host screenshots and thumbnails on your own S3 account or on
    Browshot.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshothost-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshothost-get-openapi.md
- name: Browshot - Get the HTML code
  x-api-slug: screenshothtml-get
  description: Retrieve the HTML code of the rendered page. This API call should be
    used when html=1 was specified in the screenshot request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshothtml-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshothtml-get-openapi.md
- name: Browshot - Query screenshot status
  x-api-slug: screenshotinfo-get
  description: Once a screenshot has been requested, its status must be checked until
    it is either "error" or "finished".
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotinfo-get-openapi.md
- name: Browshot - Get information about screenshots
  x-api-slug: screenshotlist-get
  description: Get information about the last 100 screenshots requested.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotlist-get-openapi.md
- name: Browshot - Request multiple screenshots
  x-api-slug: screenshotmultiple-get
  description: |-
    Request multiple screenshots in one API call. The API call accepts all the parameters supported by screenshot/create.
    You can specify up to 10 URLs and 10 instances for a total of 100 screenshots in one API call.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotmultiple-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotmultiple-get-openapi.md
- name: Browshot - Search for screenshots
  x-api-slug: screenshotsearch-get
  description: Search for screenshots of a specific URL.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotsearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotsearch-get-openapi.md
- name: Browshot - Share a screenshot
  x-api-slug: screenshotshare-get
  description: You can make your screenshots public, add notes, and share it with
    your friends and colleagues. Only screenshots which are successfully completed
    can be shared.n the thumbnail. You can take a 1024x768 screenshot, crop it to
    768x768, and get it scaled down to 300x300.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotshare-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotshare-get-openapi.md
- name: Browshot - Retrieve a thumbnail image
  x-api-slug: screenshotthumbnail-get
  description: |-
    Unlike the other API calls, this API sends back the thumbnail as a PNG file, not JSON. The HTTP response code indicates whether the screenshot was successful (200), or incomplete (404) or failed (404). If the screenshot failed or is not finished, a default image "Not found" is sent.

    You can crop your screenshots. The crop is done first, then the thumbnail. You can take a 1024x768 screenshot, crop it to 768x768, and get it scaled down to 300x300.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotthumbnail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/screenshot/master/_listings/browshot/screenshotthumbnail-get-openapi.md
x-common:
- type: x-website
  url: http://browshot.com/
- type: x-api-gallery
  url: http://broadleaf.commerce.api.gallery.streamdata.io
- type: x-api-stack
  url: http://browshot.stack.network
- type: x-base
  url: https://api.browshot.com/api/
- type: x-blog
  url: http://blog.browshot.com/
- type: x-blog-rss
  url: http://blog.browshot.com/feeds/posts/default
- type: x-crunchbase
  url: http://www.crunchbase.com/company/browshot
- type: x-crunchbase
  url: https://crunchbase.com/organization/browshot
- type: x-developer
  url: http://browshot.com/api/documentation
- type: x-email
  url: feedback@browshot.com
- type: x-twitter
  url: https://twitter.com/BrowshotCom
- type: x-website
  url: http://browshot.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---