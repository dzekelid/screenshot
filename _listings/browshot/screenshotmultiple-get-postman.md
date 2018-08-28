{
  "info": {
    "name": "Browshot Request multiple screenshots",
    "_postman_id": "32c8e7e3-fdd8-4bac-af41-9d8450c68d91",
    "description": "Request multiple screenshots in one API call. The API call accepts all the parameters supported by screenshot/create.\nYou can specify up to 10 URLs and 10 instances for a total of 100 screenshots in one API call.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Screenshot",
      "item": [
        {
          "id": "4111b869-3168-4f9b-b8a9-ff335a065120",
          "name": "CreateMultipleScreenshots",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/multiple?cache=%7B%7D&cookie=%7B%7D&delay=%7B%7D&details=%7B%7D&flash_delay=%7B%7D&headers=%7B%7D&hosting=%7B%7D&hosting_bucket=%7B%7D&hosting_file=%7B%7D&hosting_headers=%7B%7D&hosting_height=%7B%7D&hosting_scale=%7B%7D&hosting_width=%7B%7D&html=%7B%7D&instance_id=%7B%7D&max_wait=%7B%7D&post_data=%7B%7D&priority=%7B%7D&referer=%7B%7D&screen_height=%7B%7D&screen_width=%7B%7D&script=%7B%7D&size=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request multiple screenshots in one API call. The API call accepts all the parameters supported by screenshot/create.\nYou can specify up to 10 URLs and 10 instances for a total of 100 screenshots in one API call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d23fdbc-e70b-4617-b73c-db4b8ed964b1"
            }
          ]
        }
      ]
    }
  ]
}