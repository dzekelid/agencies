{
  "info": {
    "name": "Dezrez Get meeting places for an agency",
    "_postman_id": "10d2a75e-8616-4f90-af6b-f8246b4fad5d",
    "description": "Get meeting places for an agency.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "801bc453-bf6d-4c1a-9cfb-1060f50d19c6",
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
              "id": "3045063d-6640-4759-b646-96f9f0af7346"
            }
          ]
        }
      ]
    },
    {
      "name": "Branchesan",
      "item": [
        {
          "id": "ea56993b-1c94-499e-b4fd-2f9c3321422a",
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
              "id": "d685124d-1683-4b51-8635-3c0fb2a93114"
            }
          ]
        }
      ]
    },
    {
      "name": "Milestone",
      "item": [
        {
          "id": "b9d5afa2-b147-47eb-a2aa-884283fc7641",
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
              "id": "cdbbea1a-3290-493f-ac8d-501385ce2e60"
            }
          ]
        }
      ]
    },
    {
      "name": "Administratorsan",
      "item": [
        {
          "id": "24a0d710-ca78-487d-ad15-a8a7d05a4e37",
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
              "id": "31edd9b0-a28d-4934-8e1c-7736c6f63ab4"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "5af29479-aaf7-412f-84ce-91db017bbac1",
          "name": "Agency_AccountManager",
          "request": {
            "url": "http://api.dezrez.com/api/agency/accountmanager",
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
            "description": "Get the account manager for an agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "984462ce-bea1-4f13-963e-2da793d00460"
            }
          ]
        }
      ]
    },
    {
      "name": "Meeting",
      "item": [
        {
          "id": "69b226fa-8363-475a-9ac1-c5f571203a3a",
          "name": "Agency_MeetingPlaces",
          "request": {
            "url": "http://api.dezrez.com/api/agency/meetingplaces",
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
            "description": "Get meeting places for an agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bde73ca1-1104-4660-b028-5db2a8d038d0"
            }
          ]
        }
      ]
    }
  ]
}