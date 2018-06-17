{
  "info": {
    "name": "BMC Software API Get Alarm by Id",
    "_postman_id": "198197f4-82e4-4af0-868e-6413d6692f35",
    "description": "Retrieves a single alarm",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "7c14305a-ac74-4a13-8ee3-63627faade08",
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
              "id": "890919e2-94f1-46c9-bd48-bd57a033a7f5"
            }
          ]
        },
        {
          "id": "8b42e408-8967-43af-b6bf-6c38f56699b8",
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
              "id": "da61bb05-e01f-4aab-8231-1645f6b0409d"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "75f6df44-2ff9-4eb7-93ef-8ef29fd0d393",
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
              "id": "3ee9cb38-e632-4441-afbf-5af2db7fe902"
            }
          ]
        },
        {
          "id": "31ae7ea5-35b8-47d5-95e9-e613e3986544",
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
              "id": "972f5b30-8a75-4f7f-8162-5317aa2cdd48"
            }
          ]
        },
        {
          "id": "9ea7baef-338a-4335-8f0c-5493b6677943",
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
              "id": "e88c2d0b-f11c-4072-a0a9-b8b033a39709"
            }
          ]
        },
        {
          "id": "ac61babd-d7e3-454d-bf7e-52c746f14505",
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
              "id": "8de5bdaf-f518-4a19-abd9-8225cc34723d"
            }
          ]
        },
        {
          "id": "376a4579-0e0a-405b-a697-0674023e505c",
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
              "id": "cb70e692-5669-4dcb-b2b3-22eee499ebe0"
            }
          ]
        },
        {
          "id": "f9be50b4-7d4f-413f-aa5b-e453d66a8b34",
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
              "id": "0cc5b1e6-739a-4b97-a619-a359f26295a6"
            }
          ]
        },
        {
          "id": "909c164b-2f4a-4501-868e-b4b30068f980",
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
              "id": "df9792bd-b3fb-477c-a192-273333fc6db2"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "8f9ce2bc-6197-4dff-b413-41400a47b8df",
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
              "id": "21028975-2924-48b6-a93c-305ceb0f9e50"
            }
          ]
        },
        {
          "id": "31a9c39d-3f57-4293-87fa-297b500781ad",
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
              "id": "a021508b-59b0-4917-b272-8bc3ba32ab39"
            }
          ]
        }
      ]
    }
  ]
}