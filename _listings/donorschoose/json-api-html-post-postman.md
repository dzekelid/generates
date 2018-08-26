{
  "info": {
    "name": "Donors Choose Generate Gift Code",
    "_postman_id": "8b6e0e22-a55c-494c-9899-c008225ed2b4",
    "description": "Generate Gift Code",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Generate",
      "item": [
        {
          "id": "e7f769d5-964c-4259-a41b-265101945f9e",
          "name": "generate-gift-code",
          "request": {
            "url": "http://api.donorschoose.org/common/json_api.html",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Generate Gift Code"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1901f58-4771-4294-974a-09078d9ddc8e"
            }
          ]
        }
      ]
    }
  ]
}