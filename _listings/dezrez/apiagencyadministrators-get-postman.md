{
  "info": {
    "name": "Dezrez Get the administrators for an agency",
    "_postman_id": "de0f076c-6360-40f5-903c-a553c5862dcf",
    "description": "Get the administrators for an agency.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Branch",
      "item": [
        {
          "id": "799045b6-08d0-43ae-8c1b-79f31fe86598",
          "name": "Branch_AdministratorsByid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/branch/:id/administrators"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get branch administrators by its id.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80b34efa-8322-4856-b543-e50a8c3ce40b"
            }
          ]
        }
      ]
    },
    {
      "name": "Administratorsan",
      "item": [
        {
          "id": "7dcd7c41-6afc-4816-a27a-64ff3f3fb818",
          "name": "Agency_Administrators",
          "request": {
            "url": "http://api.dezrez.com/api/agency/administrators",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the administrators for an agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9df897fc-f124-4845-b8d7-7806533d95bc"
            }
          ]
        }
      ]
    }
  ]
}