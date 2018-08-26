{
  "info": {
    "name": "Instructure Canvas Polls API Get a single poll",
    "_postman_id": "7726de19-1a60-4ce1-bbed-557b4610745b",
    "description": "Get a single poll.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Polls",
      "item": [
        {
          "id": "3978bf60-45a3-479d-8b37-50e3c1c7933f",
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
              "id": "7d351eeb-0a3a-4407-8768-588fdf6adafc"
            }
          ]
        },
        {
          "id": "84c82f9c-20cf-4e54-99d8-1aee95ea26d7",
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
              "id": "1e727600-6f1b-4c10-9141-9ce4d0b1ef37"
            }
          ]
        },
        {
          "id": "a656c803-61e2-41fc-8487-af914514208b",
          "name": "get-a-single-poll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single poll."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb3887d5-1ad2-4e59-b013-0d5c69c53b0f"
            }
          ]
        },
        {
          "id": "dcb6f33a-f831-4e1e-acab-8af3f6265c27",
          "name": "delete-a-poll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a poll."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f4ff8c7-f242-4b31-bbca-db23a41ebf93"
            }
          ]
        }
      ]
    }
  ]
}