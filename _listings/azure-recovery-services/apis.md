---
name: Azure Recovery Services
x-slug: azure-recovery-services
description: Learn how to use Site Recovery for business continuity and disaster recovery
  strategy for private clouds. Tutorials and other documentation show you how to plan,
  deploy, and manage the orchestration of replicating on-premises physical servers
  and virtual machines to the cloud or to a secondary datacenter.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
x-kinRank: "10"
x-alexaRank: ""
tags: Azure Recovery Services
created: "2018-05-21"
modified: "2018-05-21"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Recovery Service API Operations List
  x-api-slug: azure-recovery-service-api
  description: Returns the list of available operations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/operations
  tags: Operations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesoperations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesoperations-get-openapi.md
- name: Azure Recovery Service API Backup Vault Configs Get
  x-api-slug: azure-recovery-service-api
  description: Fetches vault config.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/backupconfig/vaultconfig
  tags: Backup Vault Configs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamebackupconfigvaultconfig-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamebackupconfigvaultconfig-get-openapi.md
- name: Azure Recovery Service API Backup Vault Configs Update
  x-api-slug: azure-recovery-service-api
  description: Updates vault config model type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/backupconfig/vaultconfig
  tags: Backup Vault Configs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamebackupconfigvaultconfig-patch-openapi.md
- name: Azure Recovery Service API Backup Storage Configs Get
  x-api-slug: azure-recovery-service-api
  description: Fetches resource storage config.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/backupstorageconfig/vaultstorageconfig
  tags: Backup Storage Configs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamebackupstorageconfigvaultstorageconfig-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamebackupstorageconfigvaultstorageconfig-get-openapi.md
- name: Azure Recovery Service API Backup Storage Configs Update
  x-api-slug: azure-recovery-service-api
  description: Updates vault storage model type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/backupstorageconfig/vaultstorageconfig
  tags: Backup Storage Configs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamebackupstorageconfigvaultstorageconfig-patch-openapi.md
- name: Azure Recovery Service API Vault Certificates Create
  x-api-slug: azure-recovery-service-api
  description: Upload a certificate for a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/certificates/{certificateName}
  tags: Vault Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamecertificatescertificatename-put-openapi.md
- name: Azure Recovery Service API Registered Identities Delete
  x-api-slug: azure-recovery-service-api
  description: Unregisters the given container from your Recovery Services vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/registeredIdentities/{identityName}
  tags: Registered Identities
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnameregisteredidentitiesidentityname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnameregisteredidentitiesidentityname-delete-openapi.md
- name: Azure Recovery Service API Replication Usages List
  x-api-slug: azure-recovery-service-api
  description: Fetches the replication usages of the vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/replicationUsages
  tags: Replication Usages
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnamereplicationusages-get-openapi.md
- name: Azure Recovery Service API Vaults List By Subscription Id
  x-api-slug: azure-recovery-service-api
  description: Fetches all the resources of the specified type in the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/vaults
  tags: Vaults Subscription
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidprovidersmicrosoftrecoveryservicesvaults-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidprovidersmicrosoftrecoveryservicesvaults-get-openapi.md
- name: Azure Recovery Service API Vaults List By Resource Group
  x-api-slug: azure-recovery-service-api
  description: Retrieve a list of Vaults.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults
  tags: Vaults Resource Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaults-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaults-get-openapi.md
- name: Azure Recovery Service API Vaults Get
  x-api-slug: azure-recovery-service-api
  description: Get the Vault details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultname-get-openapi.md
- name: Azure Recovery Service API Vaults Create Or Update
  x-api-slug: azure-recovery-service-api
  description: Creates or updates a Recovery Services vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultname-put-openapi.md
- name: Azure Recovery Service API Vaults Delete
  x-api-slug: azure-recovery-service-api
  description: Deletes a vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultname-delete-openapi.md
- name: Azure Recovery Service API Vaults Update
  x-api-slug: azure-recovery-service-api
  description: Updates the vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}
  tags: Vaults
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultname-patch-openapi.md
- name: Azure Recovery Service API Vault Extended Info Get
  x-api-slug: azure-recovery-service-api
  description: Get the vault extended info.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/extendedInformation/vaultExtendedInfo
  tags: Vault Extended Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnameextendedinformationvaultextendedinfo-get-openapi.md
- name: Azure Recovery Service API Vault Extended Info Create Or Update
  x-api-slug: azure-recovery-service-api
  description: Create vault extended info.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/extendedInformation/vaultExtendedInfo
  tags: Vault Extended Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnameextendedinformationvaultextendedinfo-put-openapi.md
- name: Azure Recovery Service API Vault Extended Info Update
  x-api-slug: azure-recovery-service-api
  description: Update vault extended info.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/extendedInformation/vaultExtendedInfo
  tags: Vault Extended Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnameextendedinformationvaultextendedinfo-patch-openapi.md
- name: Azure Recovery Service API Usages List By Vaults
  x-api-slug: azure-recovery-service-api
  description: Fetches the usages of the vault.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com////Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/usages
  tags: Usages Vaults
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnameusages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftrecoveryservicesvaultsvaultnameusages-get-openapi.md
- name: Azure Recovery Service API
  x-api-slug: azure-recovery-service-api
  description: Learn how to use Site Recovery for business continuity and disaster
    recovery strategy for private clouds. Tutorials and other documentation show you
    how to plan, deploy, and manage the orchestration of replicating on-premises physical
    servers and virtual machines to the cloud or to a secondary datacenter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-site-recovery.png
  humanURL: https://azure.microsoft.com/en-us/services/site-recovery/
  baseURL: ://management.azure.com//
  tags: Azure Recovery Services
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-recovery-services/master/_listings/azure-recovery-services/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/site-recovery/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/site-recovery/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/site-recovery/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/site-recovery/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---