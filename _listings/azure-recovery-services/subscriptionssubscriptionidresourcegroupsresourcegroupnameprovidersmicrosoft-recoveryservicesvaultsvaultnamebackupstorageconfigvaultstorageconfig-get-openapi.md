---
swagger: "2.0"
x-collection-name: Azure Recovery Services
x-complete: 0
info:
  title: Azure Recovery Service API Backup Storage Configs Get
  version: 1.0.0
  description: Fetches resource storage config.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/operations:
    get:
      summary: Operations List
      description: Returns the list of available operations.
      operationId: Operations_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesoperations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Operations
  ? /Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/backupconfig/vaultconfig
  : get:
      summary: Backup Vault Configs Get
      description: Fetches vault config.
      operationId: BackupVaultConfigs_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnamebackupconfigvaultconfig-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Backup Vault Configs
    patch:
      summary: Backup Vault Configs Update
      description: Updates vault config model type.
      operationId: BackupVaultConfigs_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnamebackupconfigvaultconfig-patch
      parameters:
      - in: body
        name: backupVaultConfig
        description: Backup vault config
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Backup Vault Configs
  ? /Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/backupstorageconfig/vaultstorageconfig
  : get:
      summary: Backup Storage Configs Get
      description: Fetches resource storage config.
      operationId: BackupStorageConfigs_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnamebackupstorageconfigvaultstorageconfig-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Backup Storage Configs
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---