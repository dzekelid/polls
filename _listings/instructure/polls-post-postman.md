{
  "info": {
    "name": "Instructure Canvas Polls API Create a single poll",
    "_postman_id": "63568279-ee62-420f-bac0-aec8859027ba",
    "description": "Create a single poll.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Polls",
      "item": [
        {
          "id": "5c5aa7cd-bfdf-4e4a-a806-ed86ac39cd1b",
          "name": "list-polls",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/polls",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List polls."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6a55684-aafb-47ed-be36-7f8f5523b131"
            }
          ]
        },
        {
          "id": "9b80f9ba-e20e-4d01-ae3f-165fb3610a90",
          "name": "create-a-single-poll",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/polls?polls[][description]=%7B%7D&polls[][question]=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a single poll."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ccfb650-0449-436c-a5e7-4ac59a23808a"
            }
          ]
        }
      ]
    }
  ]
}