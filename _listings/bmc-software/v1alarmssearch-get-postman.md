{
  "info": {
    "name": "BMC Software API Get Alarms by Name",
    "_postman_id": "c73a3335-e11b-4294-b51d-c4c84063d9f9",
    "description": "Retrieves alarms by name",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "28f1d9a4-fcde-4ea9-b226-a601f1735a3e",
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
              "id": "e7638cda-56a8-489f-9350-9d1bf0f5bf47"
            }
          ]
        },
        {
          "id": "6b076321-02a3-4644-ab1d-10f7ee312cdf",
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
              "id": "9e23c609-4198-44d3-96c2-f9f4af93b455"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "c5c8a2ad-f767-49e1-91bc-3dfe6ffbd86f",
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
              "id": "d85eeddc-2d30-44fa-866c-e0d7aa29a976"
            }
          ]
        },
        {
          "id": "2221b6e6-29e7-42a2-a3cb-2803b1d87edc",
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
              "id": "207b400d-9244-4e23-aa1a-5322c3c338bd"
            }
          ]
        },
        {
          "id": "978399e3-2f33-44c0-84df-4f3c2385a57d",
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
              "id": "4c69bff2-dfab-49ff-a561-44bffaa0b825"
            }
          ]
        },
        {
          "id": "f6b8f219-b51e-4380-8b6e-89913de62a2a",
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
              "id": "b6e00425-a601-4476-bf61-d25fa116dca2"
            }
          ]
        },
        {
          "id": "81c5edf6-6de6-4e2c-b26c-0903068e4a6a",
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
              "id": "4e6bfab3-2002-489f-b46c-7697d95569df"
            }
          ]
        },
        {
          "id": "85ece081-57b5-48f1-b6c0-3d73c4e2d289",
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
              "id": "06577dfc-7cdc-4b26-9023-c934f767ebd7"
            }
          ]
        },
        {
          "id": "b9c85b3f-8f54-45e8-8686-a57b2da11c10",
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
              "id": "efeadf4e-8056-4070-98ca-4b79d505056a"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "14e0a08b-9c96-4789-866a-a715e4ec51ed",
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
              "id": "2530aadc-10ab-426a-b0ee-eca7508f5f54"
            }
          ]
        },
        {
          "id": "0a923193-2ab9-444d-8b33-b3199a5ae86c",
          "name": "get-alarm-by-id",
          "request": {
            "url": "http://example.com/api/v1/alarm/:alarmId?alarmId=alarmId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a single alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0126e02f-3770-4765-ad65-e396143eead9"
            }
          ]
        },
        {
          "id": "b110af01-0d9b-4f03-ac5a-3fd7844a1020",
          "name": "get-alarms-by-name",
          "request": {
            "url": "http://example.com/api/v1/alarms/search?alarmName=alarmName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves alarms by name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34e9e5dc-c149-4495-be02-ac663ba54865"
            }
          ]
        }
      ]
    }
  ]
}