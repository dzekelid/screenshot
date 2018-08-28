{
  "info": {
    "name": "Browshot Query screenshot status",
    "_postman_id": "5c362a4d-053f-4447-9f09-b099a4a9d8e8",
    "description": "Once a screenshot has been requested, its status must be checked until it is either \"error\" or \"finished\".",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "90b95dcb-d20b-4450-b3e2-f28ae2ee7b7b",
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
              "id": "231dba17-d960-4dc0-aba7-f90f9d9f74b1"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "04d332d2-58cf-4ecd-9084-eb21b7830a74",
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
              "id": "4ee00eb5-23ab-471c-8a5a-76044b93aa94"
            }
          ]
        },
        {
          "id": "62746e2a-f1e9-4ac7-a066-74b514e9db90",
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
              "id": "06618a00-3b3a-4de5-ac8f-42e2fcb04b59"
            }
          ]
        }
      ]
    },
    {
      "name": "Browser",
      "item": [
        {
          "id": "c29034f9-969f-4e27-bb6f-716d7e2431ad",
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
              "id": "6c46442e-deb9-4812-aef7-5ce7538b103b"
            }
          ]
        },
        {
          "id": "b5d36a4c-185d-4cea-b975-03a50ac41906",
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
              "id": "a2604e07-8622-4942-aa0e-af64f4b8d040"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "34827709-19bf-4704-b862-472855c1f4cb",
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
              "id": "da7cb48d-6828-4bb4-8ce7-86b982e73c7c"
            }
          ]
        },
        {
          "id": "66bed389-e188-4415-b61a-7fec13051b96",
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
              "id": "82eb6010-c579-4a90-aaa7-6aa8dea7c630"
            }
          ]
        }
      ]
    },
    {
      "name": "Screenshot",
      "item": [
        {
          "id": "881342a9-9393-46db-a6ca-942d10ba5ac4",
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
              "id": "f7b7fb1a-1804-4fea-b965-5efbfbfa4058"
            }
          ]
        },
        {
          "id": "0583c0ee-d89a-4f97-a541-5027fa14f9b2",
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
              "id": "40c616a1-05ca-40c9-87b3-90b1128613d2"
            }
          ]
        },
        {
          "id": "baa99c51-dde7-46ba-939e-9e337f35180c",
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
              "id": "56972044-e75e-4dce-b7c5-ece13beb6286"
            }
          ]
        },
        {
          "id": "4fe865ec-518b-4b6f-a5bc-e86d3f12bbe3",
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
              "id": "25df9b22-2064-4cb5-84af-17bdceef322e"
            }
          ]
        },
        {
          "id": "a7556685-dc4b-43c5-8680-b7bea51cafc1",
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
              "id": "dc5d69bf-a26b-4b38-8d1d-65c9838ed359"
            }
          ]
        }
      ]
    }
  ]
}