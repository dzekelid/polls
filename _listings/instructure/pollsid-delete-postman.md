{
  "info": {
    "name": "Instructure Canvas Polls API Delete a poll",
    "_postman_id": "8d8c8319-169c-4adf-8fb2-387b9f0cc838",
    "description": "Delete a poll.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Polls",
      "item": [
        {
          "id": "06788cf5-c854-4ac4-a1cc-7bf6c7c445f9",
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
              "id": "3d6206c7-92e7-403a-80ec-613ac44cd435"
            }
          ]
        },
        {
          "id": "057975e3-c953-4cf9-8694-c08dba6c8cc6",
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
              "id": "fe4c6d66-4012-4d4d-9684-4956b5face5e"
            }
          ]
        },
        {
          "id": "141ec767-993a-4efa-afef-daa919e104c7",
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
              "id": "ed535f56-2a5b-496c-b4ce-df40b3efdd2f"
            }
          ]
        }
      ]
    }
  ]
}