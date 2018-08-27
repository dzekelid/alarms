{
  "info": {
    "name": "BMC Software API Get Alarm by Id",
    "_postman_id": "b49385d1-bfe6-4132-8da0-33a45c5f879f",
    "description": "Retrieves a single alarm",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "aa2ac6a7-0b02-4075-9243-359b64766aa4",
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
              "id": "50e763fa-91d4-45f2-b25a-b94a968be2df"
            }
          ]
        },
        {
          "id": "0991f74a-5963-4f35-8493-55328b63408a",
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
              "id": "cb729da0-9a0d-4217-bce2-ce6561bb7b21"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "4e14a0bc-8b7c-4b62-9681-698d7a2eb650",
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
              "id": "283c89a0-4dd3-471e-b97f-55fecd1b5514"
            }
          ]
        },
        {
          "id": "32a52744-f1d3-4b64-81e2-466dae767eab",
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
              "id": "2d014d85-2c12-45cd-96a1-d30231ac2b21"
            }
          ]
        },
        {
          "id": "78f7a8a4-014d-4b71-8272-0c2591844d66",
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
              "id": "dd739a01-4437-48eb-8e94-cc46c57dac1e"
            }
          ]
        },
        {
          "id": "a25654e3-1bc5-4fa6-8c34-77081e1e5b52",
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
              "id": "731a25f1-8d95-4278-946c-15a1fcfd8d48"
            }
          ]
        },
        {
          "id": "93ac405e-4abc-454a-baa7-d14af066c2be",
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
              "id": "8d16d87e-8360-4c2f-82d8-222def0c10fa"
            }
          ]
        },
        {
          "id": "0b9c77b2-ff9a-4503-ac4c-ade9eb93ebf4",
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
              "id": "d4b5325b-ec8d-4724-9b00-08b2cb6f9089"
            }
          ]
        },
        {
          "id": "91b9d0a3-74c7-4805-8385-dc7a0735ff1d",
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
              "id": "23e8164a-f213-4e5f-a20e-dcc3889ef58f"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "05457fca-7693-45fa-90f1-31634dee9865",
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
              "id": "60e59a74-84c3-4380-8c8e-0dd8ea600b79"
            }
          ]
        },
        {
          "id": "0e713812-e7a0-4efd-b06b-2b3e81bcd94b",
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
              "id": "6e576493-3025-4585-90b7-4b46ff22e4fb"
            }
          ]
        },
        {
          "id": "55e2d0c5-5ce8-4a2b-9fdc-74eb000067fc",
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
              "id": "0d13a59a-1407-42a7-bb46-23df59abb3fe"
            }
          ]
        },
        {
          "id": "b1e545db-d541-42ab-af28-1a661b845d3c",
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
              "id": "1010ffb6-ffe6-4078-8276-80488a4e238d"
            }
          ]
        },
        {
          "id": "ff962bb8-ae90-4e7f-8358-d6c7959b7aea",
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
              "id": "63e7e8f1-dae1-41c8-b4d4-59327e4c7956"
            }
          ]
        },
        {
          "id": "4f70c0d3-1582-4069-997f-242c27aed03e",
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
              "id": "a15ac210-7a0e-46f4-8ae1-2f308a515a3f"
            }
          ]
        },
        {
          "id": "7820647e-d35f-4759-996c-077e1e852531",
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
              "id": "5029972d-5855-4bf9-b81a-97a68b2262ab"
            }
          ]
        },
        {
          "id": "4ca88c98-1a92-4d0e-a03a-19626f959370",
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
              "id": "0990d27e-99a4-4ab5-abe8-ad6fd5e6ff4d"
            }
          ]
        },
        {
          "id": "48d1b749-4485-40f3-a40b-ff03f7eea51e",
          "name": "get-alarm-by-id1",
          "request": {
            "url": "http://example.com/api/v2/alarms/:alarmId?alarmId=alarmId",
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
              "id": "f6f052bb-95bc-4277-a6ac-2463792646f7"
            }
          ]
        },
        {
          "id": "f455ff0e-ce7c-4288-8653-d7dd1f29f516",
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
              "id": "459fbbdb-c792-4586-9786-f7384e648083"
            }
          ]
        }
      ]
    }
  ]
}