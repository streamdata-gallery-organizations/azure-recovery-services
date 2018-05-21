{
  "info": {
    "name": "Azure Recovery Service API Backup Vault Configs Get",
    "_postman_id": "c7b4a90a-9040-4972-b3d5-0c3de220d3b5",
    "description": "Fetches vault config.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Operations",
      "item": [
        {
          "id": "fa5cb428-5edb-49ad-b9cb-5163e6b2ef26",
          "name": "Operations_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "Subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.RecoveryServices/operations"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of available operations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cee84217-3d61-4fae-ba0a-d19d2134f82a"
            }
          ]
        }
      ]
    },
    {
      "name": "Backup Vault Configs",
      "item": [
        {
          "id": "8abd47ee-443c-4ea9-b420-e9a00a52ae27",
          "name": "BackupVaultConfigs_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "Subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.RecoveryServices/vaults/:vaultName/backupconfig/vaultconfig"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "vaultName",
                  "value": "vaultName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches vault config."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b894f05a-811c-40aa-b774-a929d01dc556"
            }
          ]
        }
      ]
    }
  ]
}