{
  "info": {
    "name": "Browshot Host thumbnails on your own S3 account or on Browshot.",
    "_postman_id": "bcd681d9-762e-4fd6-85c2-76ae6ed6422d",
    "description": "You can host screenshots and thumbnails on your own S3 account or on Browshot.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "d026685a-eb6f-499e-9e79-0eb1aeeae9e8",
          "name": "GetAccountInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/account/info?details=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b96ec62e-35b3-4135-96b6-7252b79d3fe4"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "596cc657-1c9a-4dfb-8bab-f31cc4675da8",
          "name": "CreateBatch",
          "request": {
            "url": "http://api.browshot.com/api/v1/batch/ceate?hosting=%7B%7D&hosting_bucket=%7B%7D&hosting_file=%7B%7D&hosting_headers=%7B%7D&hosting_height=%7B%7D&hosting_scale=%7B%7D&hosting_width=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "cookie",
                  "value": "{}",
                  "disabled": false,
                  "description": "set a cookie for the URL requested (see Custom POST Data, Referer and Cookie) Cookies should be separated by a ; - paid screenshots only"
                },
                {
                  "key": "delay",
                  "value": "{}",
                  "disabled": false,
                  "description": "number of seconds to wait after the page has loaded"
                },
                {
                  "key": "details",
                  "value": "{}",
                  "disabled": false,
                  "description": "level of information available with screenshot/info"
                },
                {
                  "key": "file",
                  "value": "{}",
                  "disabled": false,
                  "description": "text file to use"
                },
                {
                  "key": "flash_delay",
                  "value": "{}",
                  "disabled": false,
                  "description": "number of seconds to wait after the page has loaded if Flash elements are present"
                },
                {
                  "key": "format",
                  "value": "{}",
                  "disabled": false,
                  "description": "image as PNG or JPEG"
                },
                {
                  "key": "headers",
                  "value": "{}",
                  "disabled": false,
                  "description": "any custom HTTP headers"
                },
                {
                  "key": "height",
                  "value": "{}",
                  "disabled": false,
                  "description": "thumbnail height"
                },
                {
                  "key": "html",
                  "value": "{}",
                  "disabled": false,
                  "description": "saves the HTML of the rendered page which can be retrieved by the API call screenshot/html"
                },
                {
                  "key": "instance_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "instance ID to use"
                },
                {
                  "key": "max_wait",
                  "value": "{}",
                  "disabled": false,
                  "description": "maximum number of seconds to wait before triggering the PageLoad event"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "name of the batch"
                },
                {
                  "key": "post_data",
                  "value": "{}",
                  "disabled": false,
                  "description": "send a POST requests with post_data, useful for filling out forms - paid screenshots only"
                },
                {
                  "key": "priority",
                  "value": "{}",
                  "disabled": false,
                  "description": "assign priority to the screenshot (for private instances only)"
                },
                {
                  "key": "referer",
                  "value": "{}",
                  "disabled": false,
                  "description": "use a custom referrer header - paid screenshots only"
                },
                {
                  "key": "screen_height",
                  "value": "{}",
                  "disabled": false,
                  "description": "height of the browser window"
                },
                {
                  "key": "screen_width",
                  "value": "{}",
                  "disabled": false,
                  "description": "width of the browser window"
                },
                {
                  "key": "script",
                  "value": "{}",
                  "disabled": false,
                  "description": "URL of javascript file to execute after the page load event"
                },
                {
                  "key": "size",
                  "value": "{}",
                  "disabled": false,
                  "description": "screenshots size - screen (default) or page"
                },
                {
                  "key": "width",
                  "value": "{}",
                  "disabled": false,
                  "description": "thumbnail width"
                }
              ]
            },
            "description": "Get hundreds or thousands of screenshots from a text file. You can use this API call or the dashboard. Unlike the other API calls, you must issue a POST request with the Content-Type \"multipart/form-data\" in order to upload the text file. The text file must contain the list of URLs to request, 1 URL per line. Failed screenshots will be tried up to 3 times before giving up."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79966365-a096-4bc1-9679-c0d669d87e20"
            }
          ]
        },
        {
          "id": "378a7481-8099-4441-ae45-af22056b1edb",
          "name": "GetBatchInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/batch/info?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the status of a batch requested through the API or through the dashboard."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01e027b0-419e-407b-a010-3aab468b507b"
            }
          ]
        }
      ]
    },
    {
      "name": "Browser",
      "item": [
        {
          "id": "4c1cbcc9-0a3e-4a3f-ac37-613f4cbd1b26",
          "name": "GetBrowserInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/browser/info?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a browser."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0e891e3-0da7-4064-9bea-899063d8c5d7"
            }
          ]
        },
        {
          "id": "279ca601-a39c-4b5c-a0d4-4e7661bc0690",
          "name": "GetBrowsersInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/browser/list",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all browsers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56c187bd-9269-4035-b6d0-9d478aa71ddc"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "11f170f1-0415-409e-9420-0bebab0aa979",
          "name": "GetInstanceInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/instance/info?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about an instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3dab9767-7707-415f-993a-649e21b78df7"
            }
          ]
        },
        {
          "id": "95c5cb06-02e1-4585-afd8-e762448c09b6",
          "name": "GetInstancesInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/instance/list",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79279daf-a0a4-4342-a7ad-54445467c409"
            }
          ]
        }
      ]
    },
    {
      "name": "Screenshot",
      "item": [
        {
          "id": "705d4723-2118-4815-93ec-c4c5dc493289",
          "name": "CreateScreenshot",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/create?cache=%7B%7D&cookie=%7B%7D&delay=%7B%7D&details=%7B%7D&flash_delay=%7B%7D&headers=%7B%7D&hosting=%7B%7D&hosting_bucket=%7B%7D&hosting_file=%7B%7D&hosting_headers=%7B%7D&hosting_height=%7B%7D&hosting_scale=%7B%7D&hosting_width=%7B%7D&html=%7B%7D&instance_id=%7B%7D&max_wait=%7B%7D&post_data=%7B%7D&priority=%7B%7D&referer=%7B%7D&screen_height=%7B%7D&screen_width=%7B%7D&script=%7B%7D&shots=%7B%7D&shot_interval=%7B%7D&size=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Screenshots requests to private and shared instances require a positive balance.\n\n*IMPORTANT*: Remember that you can only do 100 free screenshots per month. To used a premium instance, use instance_id=65 for example."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb596336-f7a2-46e9-b8f6-868a4a795454"
            }
          ]
        },
        {
          "id": "e376eca4-4fe5-4a28-a392-48d39cc1324b",
          "name": "DeleteScreenshot",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/delete?data=%7B%7D&id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can delete details of your screenshots to remove any confidential information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46f9c467-e95f-4699-86b6-2ea2715d8a72"
            }
          ]
        },
        {
          "id": "e7ca5b73-b562-4b8f-b3c6-dd84c4b1f982",
          "name": "HostScreenshot",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/host?bucket=%7B%7D&file=%7B%7D&headers=%7B%7D&height=%7B%7D&hosting=%7B%7D&id=%7B%7D&scale=%7B%7D&width=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can host screenshots and thumbnails on your own S3 account or on Browshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e15a080a-352a-4e3d-bb71-2e95a630ac86"
            }
          ]
        }
      ]
    }
  ]
}