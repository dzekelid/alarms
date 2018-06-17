{
  "info": {
    "name": "BMC Software API Create Alarm",
    "_postman_id": "32af937f-f775-4b1e-8354-2d5635bd200c",
    "description": "Create an Alarm",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "6ef5c547-b649-4f19-bedd-aba92a1d4a53",
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
              "id": "56278648-f2d9-4ce0-a2ee-00e3315465b0"
            }
          ]
        },
        {
          "id": "be1cd714-d67c-44d0-ac99-0c0f324522e8",
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
              "id": "6c3e5567-c2de-4bdd-86a6-d4e1239d9f96"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "d6bd20ea-953d-4f4a-a3da-6e69e9e52af6",
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
              "id": "46981862-9d64-4224-9e0f-1fe5e8a33a71"
            }
          ]
        },
        {
          "id": "2ed9506c-c4eb-4b66-a103-49dff435cb9f",
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
              "id": "e4001142-cb18-4aa1-a411-658954d00d6f"
            }
          ]
        },
        {
          "id": "3265d277-b7af-46bd-8076-98aa66024875",
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
              "id": "c1fd8757-2186-44e8-8098-7e0d8fe95de9"
            }
          ]
        },
        {
          "id": "8246d1f7-4ce3-48f4-a95d-df24f6396bc9",
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
              "id": "050253a0-7f7d-4e4e-9fa2-236ce5973e38"
            }
          ]
        },
        {
          "id": "393285af-0db6-4784-863a-4549ea21768e",
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
              "id": "381426e4-d862-4f0b-bbdb-5c94bcac9d8d"
            }
          ]
        },
        {
          "id": "d0396a9c-e56b-4326-b8c4-a1ad91d6f608",
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
              "id": "a9a62505-c7e8-45b0-bd32-2ecb27cdabb5"
            }
          ]
        },
        {
          "id": "8fa407ff-b422-4e47-963b-c2bc63185519",
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
              "id": "5869aaea-feae-45d8-8cb0-3d33f922750b"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "ffb34ae0-a49e-4ad0-81fc-6cd3faee7952",
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
              "id": "f135c937-7ca1-4610-a200-869bcefbb185"
            }
          ]
        },
        {
          "id": "2c9f5279-3f0f-4c42-9d08-43dd72de6f6e",
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
              "id": "db0fe2c2-3c55-43d3-acfd-1895e48981b7"
            }
          ]
        },
        {
          "id": "cc20bc00-07f4-465c-8994-4980854a2822",
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
              "id": "48801a6c-841c-40c9-9b72-9e3523307795"
            }
          ]
        },
        {
          "id": "ecc2546a-03f1-4350-8f4c-b68c1d792958",
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
              "id": "0cff1a41-09ac-41ca-acac-606823416b9e"
            }
          ]
        },
        {
          "id": "39e70a93-bd03-483a-9300-658add1874b9",
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
              "id": "086126dc-7774-4cec-9fbe-c4a6d9d6633c"
            }
          ]
        },
        {
          "id": "89a1794d-570e-42ee-a2e3-aa52c6f476d3",
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
              "id": "56283056-67fd-41a9-bba6-d66346ecf92e"
            }
          ]
        },
        {
          "id": "9211a96a-483f-4d38-987e-83e46a21c6af",
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
              "id": "040d586d-9149-41a7-b442-782c30a963de"
            }
          ]
        }
      ]
    }
  ]
}