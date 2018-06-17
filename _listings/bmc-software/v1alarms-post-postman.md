{
  "info": {
    "name": "BMC Software API Create Alarm",
    "_postman_id": "b7cddbd5-e621-4202-80ce-5b49585f1a29",
    "description": "Create an Alarm",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "0bddbcda-b681-42dd-a70d-5bd7eee46b1c",
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
              "id": "5e3cda8a-1192-4703-a1f0-6caff1fb81ee"
            }
          ]
        },
        {
          "id": "72639a82-7548-4942-a39d-c7e666686b26",
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
              "id": "d08e470c-8ed0-4424-a974-731dedd2c81e"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "ce112585-9827-4aab-8ac1-bb0bb42edc51",
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
              "id": "09d2337e-2e7c-4db4-9074-c1de3aecdf50"
            }
          ]
        },
        {
          "id": "81859ccc-027b-400f-bbfa-3918e9886636",
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
              "id": "581882af-8067-4fbc-a5e1-ee8bf00153a8"
            }
          ]
        },
        {
          "id": "e8fb4d62-a8e3-41ef-9910-ee5468b01a6b",
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
              "id": "fda0ce85-2f0d-47af-8f5f-10d5ba92f694"
            }
          ]
        },
        {
          "id": "90a28c68-a2e1-47ce-9f02-5ac26501b480",
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
              "id": "c127c14b-7e18-4f06-af4f-72ea5a713905"
            }
          ]
        },
        {
          "id": "1c8e5ecf-fc54-464c-98c3-198f66f1f61e",
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
              "id": "9f135e16-d97e-4125-a19f-d05d6e05d2bd"
            }
          ]
        },
        {
          "id": "12cc4fd2-ba79-4d1b-aa27-8468c39d5f2c",
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
              "id": "39c5e76e-b906-4a3c-a8d3-f2b248cd5141"
            }
          ]
        },
        {
          "id": "3d92d292-0e47-494f-a5ea-1f17762f7d00",
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
              "id": "d77f60cd-5683-4a9c-9be2-cfb17a6b2247"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "a0fb3ef7-b993-406f-a425-10c862f72665",
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
              "id": "12104915-a246-4a8f-a406-e09eda542463"
            }
          ]
        },
        {
          "id": "33b6c7ef-f708-4b5c-afc8-67076c5fb555",
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
              "id": "cbff1ea3-ce32-4e80-b506-344db1856e47"
            }
          ]
        },
        {
          "id": "ef727324-f9e3-4640-a66f-3828b8f3dfb2",
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
              "id": "61d7f4d3-3826-46b3-9923-35ba848b8e28"
            }
          ]
        },
        {
          "id": "03ab9c9d-0b8a-4416-ac27-61a5372f5905",
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
              "id": "25811215-968e-4ab6-ba91-228ec13ac317"
            }
          ]
        }
      ]
    }
  ]
}