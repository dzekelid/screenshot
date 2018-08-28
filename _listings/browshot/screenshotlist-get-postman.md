{
  "info": {
    "name": "Browshot Get information about screenshots",
    "_postman_id": "fcf3575d-a57f-4659-8e5e-c21446a855e0",
    "description": "Get information about the last 100 screenshots requested.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "d07b5913-956f-468c-a689-4a77ce0d006a",
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
              "id": "6210ccf7-2611-4b3b-910f-d2ea94f80720"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "1cae9c00-3e64-4555-a748-2f974bd77b7b",
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
              "id": "4e82524c-9fbe-41f2-9ad0-64ec606de196"
            }
          ]
        },
        {
          "id": "ab1ec578-a0c7-438d-aec1-1579251fb26f",
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
              "id": "70838ed2-a499-42d4-9526-93cc487b5732"
            }
          ]
        }
      ]
    },
    {
      "name": "Browser",
      "item": [
        {
          "id": "464d771a-9aa5-4104-bb2c-aa2190aa6ccc",
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
              "id": "d87468e4-c6e4-4148-8d55-02adaa4edaf5"
            }
          ]
        },
        {
          "id": "56f7deec-99c7-4772-8eaa-0d0e070b2fb7",
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
              "id": "cb9bda88-99fa-401a-9442-4c1acad92a0d"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "da4d8f06-3521-464b-b39e-5a59c948811a",
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
              "id": "998d9fa9-c61c-4f62-be1a-870c520c690c"
            }
          ]
        },
        {
          "id": "04a5ed4c-2eff-41b0-9e92-e455ff4eaef2",
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
              "id": "56e27b1f-bdcc-4620-bd58-e628e3cd6b0d"
            }
          ]
        }
      ]
    },
    {
      "name": "Screenshot",
      "item": [
        {
          "id": "f9918d12-c2c8-4911-85cd-2637739111cc",
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
              "id": "f52a0de0-03b6-44c5-8518-f67a5421c245"
            }
          ]
        },
        {
          "id": "97c04800-7a99-40b8-bacd-4516d576ecbc",
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
              "id": "b6e17ac7-f105-4f27-8f1d-17df8b75d988"
            }
          ]
        },
        {
          "id": "1fdcfe6e-6ae0-45d6-b6aa-c4d4eac08ca7",
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
              "id": "293a0bfc-0215-4761-a27b-d321edd4b0aa"
            }
          ]
        },
        {
          "id": "6dde69fc-0581-4c4a-a309-2c4ae54ecdec",
          "name": "GetHTML",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/html?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the HTML code of the rendered page. This API call should be used when html=1 was specified in the screenshot request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fef439f-5b7f-44eb-a2b0-ca5d131097c4"
            }
          ]
        },
        {
          "id": "c3005e1b-644c-4d3d-825d-a0e04cfac13b",
          "name": "GetScreenshotInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/info?details=%7B%7D&id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Once a screenshot has been requested, its status must be checked until it is either \"error\" or \"finished\"."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7f70f14-d093-4b6f-ab8a-bf07e3e5c224"
            }
          ]
        },
        {
          "id": "939cee3d-b98e-4132-9e93-f76526680d2b",
          "name": "GetMultipleScreenshotsInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/list?limit=%7B%7D&status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about the last 100 screenshots requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02f4c8c1-f04a-4efb-b8d5-17e4750a6a5c"
            }
          ]
        }
      ]
    }
  ]
}