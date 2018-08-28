{
  "info": {
    "name": "Browshot Delete screenshot data",
    "_postman_id": "fe480b25-6bcb-423c-84d2-8741a1c53f32",
    "description": "You can delete details of your screenshots to remove any confidential information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "734242f4-7463-4e12-94e0-3f161dded8f0",
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
              "id": "56fe4a84-4ad0-4171-8363-37f592062b88"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "af47b1ac-af29-4f8f-8d28-09dae18c4b3b",
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
              "id": "754db03b-a499-415b-a6c9-7ca8e5928f44"
            }
          ]
        },
        {
          "id": "54a93021-5f5a-4150-9de1-370e2b58652b",
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
              "id": "f5f7b6b6-18cf-4502-99d1-9a5e001edb6c"
            }
          ]
        }
      ]
    },
    {
      "name": "Browser",
      "item": [
        {
          "id": "b8292089-3532-4877-99e6-6acb76964737",
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
              "id": "9f811c90-69e3-4b70-96ba-22f815494934"
            }
          ]
        },
        {
          "id": "56970d49-b27d-4429-b108-2303b8411da4",
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
              "id": "e76c65df-f16f-44df-878d-f864686ec442"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "fd45c105-3b05-41f9-9f06-c2172a9b44cd",
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
              "id": "2c433847-6d0b-4ff7-9fb6-659d6c027e92"
            }
          ]
        },
        {
          "id": "f938bc4d-87f8-47d8-aafe-d5ed68381775",
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
              "id": "88d5c5b6-a629-4b52-9c1c-0ac8c6e09ae1"
            }
          ]
        }
      ]
    },
    {
      "name": "Screenshot",
      "item": [
        {
          "id": "49633390-22d2-46e9-96a5-e6e8498d86c3",
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
              "id": "b3da3113-962a-4d16-a3e4-b1c7364e163e"
            }
          ]
        },
        {
          "id": "de583731-7c5f-4269-aa4e-271756354eef",
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
              "id": "8a58d7e9-e7d8-4792-b920-ed14280512b2"
            }
          ]
        }
      ]
    }
  ]
}