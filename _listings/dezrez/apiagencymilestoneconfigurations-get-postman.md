{
  "info": {
    "name": "Dezrez Get the milestone configurations for an agency",
    "_postman_id": "d4fe6ca4-e683-4988-8bd4-82f62f36b445",
    "description": "Get the milestone configurations for an agency.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "58684aff-ba1c-4bcb-8fac-0151fbf76c04",
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
              "id": "d7f192a0-c522-46fa-8f8c-138869c0a47e"
            }
          ]
        }
      ]
    },
    {
      "name": "Branchesan",
      "item": [
        {
          "id": "2be28f2c-cdac-4517-824a-d13d7946f4d6",
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
              "id": "e3fabf10-a1ea-4201-9e5f-78575f5737f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Milestone",
      "item": [
        {
          "id": "6ddac0de-9d11-4b70-9217-ddffbb70125d",
          "name": "Agency_MilestoneConfigurations",
          "request": {
            "url": "http://api.dezrez.com/api/agency/milestoneconfigurations",
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
            "description": "Get the milestone configurations for an agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9989b0ce-0d67-4a68-815b-13f1962106a0"
            }
          ]
        }
      ]
    }
  ]
}