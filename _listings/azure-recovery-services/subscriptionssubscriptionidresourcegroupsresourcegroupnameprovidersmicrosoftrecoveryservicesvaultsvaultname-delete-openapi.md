---
swagger: "2.0"
x-collection-name: Azure Recovery Services
x-complete: 0
info:
  title: Azure Recovery Service API Vaults Delete
  version: 1.0.0
  description: Deletes a vault.
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesoperations-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamebackupconfigvaultconfig-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamebackupconfigvaultconfig-patch
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamebackupstorageconfigvaultstorageconfig-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Backup Storage Configs
    patch:
      summary: Backup Storage Configs Update
      description: Updates vault storage model type.
      operationId: BackupStorageConfigs_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamebackupstorageconfigvaultstorageconfig-patch
      parameters:
      - in: body
        name: backupStorageConfig
        description: Backup storage config
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Backup Storage Configs
  ? /Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/certificates/{certificateName}
  : put:
      summary: Vault Certificates Create
      description: Upload a certificate for a resource.
      operationId: VaultCertificates_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamecertificatescertificatename-put
      parameters:
      - in: path
        name: certificateName
        description: Certificate friendly name
      - in: body
        name: certificateRequest
        description: Input parameters for uploading the vault certificate
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vault Certificates
  ? /Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/registeredIdentities/{identityName}
  : delete:
      summary: Registered Identities Delete
      description: Unregisters the given container from your Recovery Services vault.
      operationId: RegisteredIdentities_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnameregisteredidentitiesidentityname-delete
      parameters:
      - in: path
        name: identityName
        description: Name of the protection container to unregister
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Registered Identities
  ? /Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/replicationUsages
  : get:
      summary: Replication Usages List
      description: Fetches the replication usages of the vault.
      operationId: ReplicationUsages_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamereplicationusages-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Replication Usages
  /subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/vaults:
    get:
      summary: Vaults List By Subscription Id
      description: Fetches all the resources of the specified type in the subscription.
      operationId: Vaults_ListBySubscriptionId
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftrecoveryservicesvaults-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vaults Subscription
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults:
    get:
      summary: Vaults List By Resource Group
      description: Retrieve a list of Vaults.
      operationId: Vaults_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaults-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vaults Resource Group
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}:
    get:
      summary: Vaults Get
      description: Get the Vault details.
      operationId: Vaults_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultname-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vaults
    put:
      summary: Vaults Create Or Update
      description: Creates or updates a Recovery Services vault.
      operationId: Vaults_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultname-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: vault
        description: Recovery Services Vault to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Vaults
    delete:
      summary: Vaults Delete
      description: Deletes a vault.
      operationId: Vaults_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultname-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vaults
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