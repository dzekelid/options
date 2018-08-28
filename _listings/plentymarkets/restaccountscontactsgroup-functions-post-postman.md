{
  "info": {
    "name": "Plentymarkets Apply selected group function options for given contact IDs",
    "_postman_id": "870d11c3-3711-4c62-b839-05d4393aac2a",
    "description": "Applies selected group function options for given contact IDs.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Apply",
      "item": [
        {
          "id": "c6628dd8-a158-4b3a-bc11-2a43ffec93a8",
          "name": "postRestAccountsContactsGroupFunctions",
          "request": {
            "url": "http://example.com/rest/accounts/contacts/group_functions?addressLabelTemplate=%7B%7D&contactList=%7B%7D&emailTemplate=%7B%7D&newsletter=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Applies selected group function options for given contact IDs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4a9bd88-967f-4417-bf52-c08ef0caabf8"
            }
          ]
        }
      ]
    }
  ]
}