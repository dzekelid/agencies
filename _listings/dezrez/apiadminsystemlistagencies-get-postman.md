{
  "info": {
    "name": "Dezrez Lists the name and ID of all agencies in the system.",
    "_postman_id": "22ffeb01-8e3c-4385-ba1a-b28a8d3c4c77",
    "description": "Lists the name and id of all agencies in the system..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "67d6e54f-72c1-4970-9b4c-66f34ef159c9",
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
              "id": "80cef5b6-6749-4019-8131-2aeb596a7ac1"
            }
          ]
        }
      ]
    }
  ]
}