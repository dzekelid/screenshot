{
  "info": {
    "name": "link.fish Generate screenshot (browser)",
    "_postman_id": "e174ddf9-09af-45e0-a4df-6c7a500dcd27",
    "description": "Visits the URL with full browser and creates a screenshot. This request costs 5 credits.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Urls",
      "item": [
        {
          "id": "56027d0d-f7ab-4274-bcc6-06474da93588",
          "name": "Urls.browser_data.get",
          "request": {
            "url": "http://api.link.fish/Urls/browser-data?item_format=%7B%7D&screenshot=%7B%7D&screenshot_file_format=%7B%7D&screenshot_width=%7B%7D&simplify_special_types=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Visits the URL with a full browser and extracts the data. This request costs 5 credits."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a54436a5-7614-407d-a78a-c902e411b591"
            }
          ]
        },
        {
          "id": "acbe3a50-84ec-4224-9d6a-a80ad0368ad8",
          "name": "Urls.browser_screenshot.get",
          "request": {
            "url": "http://api.link.fish/Urls/browser-screenshot?file_format=%7B%7D&type=%7B%7D&url=%7B%7D&width=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Visits the URL with full browser and creates a screenshot. This request costs 5 credits."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a3cda2c-09d1-4cf7-9ed2-2a3845d56ea6"
            }
          ]
        }
      ]
    }
  ]
}