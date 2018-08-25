{
  "info": {
    "name": "Dezrez Get the branches for an agency",
    "_postman_id": "2cbace22-a43e-45a3-a6d6-46b95ded0e54",
    "description": "Get the branches for an agency.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "6dc67dfd-798b-40e6-8969-06cf737d670b",
          "name": "System_ListAgenciesByincludeSuspended",
          "request": {
            "url": "http://api.dezrez.com/api/admin/system/ListAgencies?includeSuspended=%7B%7D",
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
            "description": "Lists the name and id of all agencies in the system.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0be68b9-7b66-4d1e-8b3a-4a3a388519b8"
            }
          ]
        }
      ]
    },
    {
      "name": "Branchesan",
      "item": [
        {
          "id": "02e4900d-faee-4478-9b5c-a43dcf6a3ae3",
          "name": "Agency_Branches",
          "request": {
            "url": "http://api.dezrez.com/api/agency/branches",
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
            "description": "Get the branches for an agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "051a060a-05fe-4e60-b6e8-a307ddb1755c"
            }
          ]
        }
      ]
    }
  ]
}