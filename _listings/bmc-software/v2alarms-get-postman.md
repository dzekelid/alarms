{
  "info": {
    "name": "BMC Software API Get All Alarms",
    "_postman_id": "ac291bfd-4819-4985-9648-47172a671f02",
    "description": "Get all of the Alarms",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "45d0be82-97c9-4e0c-8e2d-302206e2db16",
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
              "id": "55a9142b-c7b7-4734-8617-f7cfbb9b20ee"
            }
          ]
        },
        {
          "id": "632bcfed-fa79-4b60-a9b4-c5f1fe0ed67f",
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
              "id": "7f0873d4-dfac-4edb-bd6b-a889f3925b41"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "8ee872c3-0822-45eb-8fc3-82c666ad1c7e",
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
              "id": "06111e54-4bf6-4f09-bbdc-5eb43e73186c"
            }
          ]
        },
        {
          "id": "9fdc768e-1740-4ce4-9cec-19448df251ee",
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
              "id": "35ea5453-cf9a-41e3-bd35-eee0aa058681"
            }
          ]
        },
        {
          "id": "ee51f35c-d6d0-4144-9e74-7db290005b6b",
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
              "id": "18ef0da0-5aa5-4ab4-8ad1-944cd651c8e4"
            }
          ]
        },
        {
          "id": "e7344d4c-0f54-4595-a4c6-181afe87a3b8",
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
              "id": "c6e0932f-b8f5-411c-ba11-0d4c8524e74c"
            }
          ]
        },
        {
          "id": "32f53565-d866-4468-983e-da98a8d09ac7",
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
              "id": "e9604793-9537-4e84-8b07-44ecde0b3f00"
            }
          ]
        },
        {
          "id": "240c047e-31b1-44e5-89b2-1556ba9fd2a3",
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
              "id": "62853814-9884-489b-bb6d-5175c9c64eed"
            }
          ]
        },
        {
          "id": "4a1cf575-d51c-47a8-87c2-8dc6971c4b95",
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
              "id": "d50d8514-52fd-4725-92f4-3b97b8ba6f1b"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "c6649f43-41c7-470c-b875-51d5cbf86480",
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
              "id": "31aa8b04-00de-45a0-9490-4c8f80eeaf70"
            }
          ]
        },
        {
          "id": "ad6751e5-6fa1-4fd8-bac1-d862e50a12a4",
          "name": "create-alarm",
          "request": {
            "url": "http://example.com/api/v1/alarms",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "name",
                  "disabled": false,
                  "description": "The name of the alarm"
                }
              ]
            },
            "description": "Create an Alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d1b8eff-0597-4162-b463-e36370898273"
            }
          ]
        },
        {
          "id": "5ff27f1a-5df6-47c5-99a4-2713ed0edca1",
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
              "id": "e6826465-4099-469c-aee6-749d0a039096"
            }
          ]
        },
        {
          "id": "921e8eea-3bd8-42de-a104-41394fe6aa56",
          "name": "update-alarm",
          "request": {
            "url": "http://example.com/api/v1/alarm/:alarmId",
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "name",
                  "disabled": false,
                  "description": "The name of the alarm"
                }
              ]
            },
            "description": "Update an Alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57cb88fb-dc1b-4c3e-bde1-65d3819b60ee"
            }
          ]
        },
        {
          "id": "5ad9f609-664b-4864-bd16-f13b8e8127b9",
          "name": "delete-alarm",
          "request": {
            "url": "http://example.com/api/v1/alarm/:alarmId?alarmId\nThe alarm to delete=alarmId%0AThe%20alarm%20to%20delete",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25465333-90bb-43fe-ae7d-157bc6804df7"
            }
          ]
        },
        {
          "id": "0df9f294-3117-446c-8afd-aab06f584434",
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
              "id": "14372987-2270-43a4-b8fd-b1f28a61f778"
            }
          ]
        },
        {
          "id": "324c17c2-8621-4325-badf-31d256306037",
          "name": "get-all-alarms1",
          "request": {
            "url": "http://example.com/api/v2/alarms",
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
              "id": "e22ed1e9-600c-4b80-ae22-5e0ebaeb6662"
            }
          ]
        },
        {
          "id": "22546053-f80d-40bb-9220-9c97cd5b995f",
          "name": "create-alarm",
          "request": {
            "url": "http://example.com/api/v2/alarms",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an Alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5aa83e2-7bd2-4e75-aba4-69e7ceac7b45"
            }
          ]
        },
        {
          "id": "84b88a0b-221d-452b-bb26-ef0381066108",
          "name": "update-alarm",
          "request": {
            "url": "http://example.com/api/v2/alarms/:alarmId?alarmId integer\nThe alarm to update=alarmId%20integer%0AThe%20alarm%20to%20update",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c008ef9e-c4c8-40a9-9027-56805750334f"
            }
          ]
        }
      ]
    }
  ]
}