{
  "info": {
    "name": "BMC Software API Get All Alarms",
    "_postman_id": "e7c198e7-c517-4d82-b05e-145035fbc154",
    "description": "Get all of the Alarms",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "8e1756ef-75ca-4511-9cb6-7dabe23a4fe1",
          "name": "information-about-the-authorized-account",
          "request": {
            "url": "http://example.com/api/account",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Information about the authorized account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d851878f-4939-4ffb-906b-ee9e4e3efef8"
            }
          ]
        },
        {
          "id": "16e1cc76-b994-4f64-bc75-eb365baedbd2",
          "name": "get-aws-integration-status",
          "request": {
            "url": "http://example.com/api/v1/account/aws/status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets AWS status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44333a64-9d6d-40a8-88b7-3969fd3667c4"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "5838636b-9944-4737-a3e0-55f632652f01",
          "name": "get-all-available-action-types",
          "request": {
            "url": "http://example.com/api/v1/actions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all known action types"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e89c322-8693-47d9-a6cf-b960a6d6ea79"
            }
          ]
        },
        {
          "id": "6815e315-75e6-462d-8900-8fe18ea0a0bd",
          "name": "get-all-installed-actions",
          "request": {
            "url": "http://example.com/api/v1/actions/installed",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all actions that are installed for the project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "472dec9c-7d68-415e-ba13-78c3a079a941"
            }
          ]
        },
        {
          "id": "239bc5af-2374-44be-b8f6-bd004387f3fe",
          "name": "install-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Installs an action"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd183277-4fc1-4349-ac6a-25259c57ae32"
            }
          ]
        },
        {
          "id": "9a702472-83e3-4b37-894d-0782d062157e",
          "name": "get-details-of-an-installed-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId?actionId\nName of plugin=actionId%0AName%20of%20plugin",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a single action definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58e158b8-ea77-4ead-9471-e571f722fdbd"
            }
          ]
        },
        {
          "id": "5b1e9b5e-bae3-43ac-b457-71ed1388e6e6",
          "name": "uninstall-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Uninstalls an action and remove it from the associated alarms(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19099827-bb32-4e26-bc6a-d5b0b1f0abf4"
            }
          ]
        },
        {
          "id": "b5198bf3-8edf-4954-9c42-63908467e0e1",
          "name": "get-all-alarms-using-an-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId/alarms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get alarms that are using this action installed for the project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ff1e5e1-7fa0-4b9b-b450-cf74ce97bf82"
            }
          ]
        },
        {
          "id": "006cd64a-b6c1-4bb1-9b8b-3f36ac0c7c1d",
          "name": "get-action",
          "request": {
            "url": "http://example.com/api/v1/actions/:action?action\nName of plugin=action%0AName%20of%20plugin",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a single action type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d69d7773-2251-4251-827f-4ea0c4d7b670"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "30b81bee-096a-417a-8f8f-b5e1c3feb1a6",
          "name": "get-all-alarms",
          "request": {
            "url": "http://example.com/api/v1/alarms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all of the Alarms"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb6aaa89-4fd2-4ac6-bbf7-11245d70d378"
            }
          ]
        }
      ]
    }
  ]
}