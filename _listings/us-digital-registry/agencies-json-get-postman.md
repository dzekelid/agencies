{
  "info": {
    "name": "U.S. Digital Registry Agency API",
    "_postman_id": "42a43fbf-0329-417d-816e-ce620ad17949",
    "description": "Provides access to a list of federal agencies.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "agencies",
      "item": [
        {
          "id": "9ecb6754-de54-4486-a996-6423fa480f6f",
          "name": "Api::V1::Agencies#index",
          "request": {
            "url": "http://usdigitalregistry.digitalgov.gov/api/v1/agencies.json?no_accounts=no_accounts&page=%7B%7D&page_size=%7B%7D&q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This lists all active agencies in the system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b83edafe-f7d9-4842-83cb-bcb2113e123c"
            }
          ]
        }
      ]
    }
  ]
}