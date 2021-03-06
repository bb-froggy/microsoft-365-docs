---
title: AppFileEvents table in the advanced hunting schema
description: Learn about file-related events associated with cloud apps and services in the AppFileEvents table of the advanced hunting schema
keywords: advanced hunting, threat hunting, cyber threat hunting, microsoft threat protection, microsoft 365, mtp, m365, search, query, telemetry, schema reference, kusto, table, column, data type, description, AppFileEvents, Cloud App Security, MCAS
search.product: eADQiWindows 10XVcnh
search.appverid: met150
ms.prod: microsoft-365-enterprise
ms.mktglfcycl: deploy
ms.sitesec: library
ms.pagetype: security
f1.keywords:
- NOCSH
ms.author: lomayor
author: lomayor
ms.localizationpriority: medium
manager: dansimp
audience: ITPro
ms.collection: M365-security-compliance 
ms.topic: article
---

# AppFileEvents

**Applies to:**
- Microsoft Threat Protection

The `AppFileEvents` table in the [advanced hunting](advanced-hunting-overview.md) schema contains information about file-related activities in cloud apps and services monitored by Microsoft Cloud App Security. Use this reference to construct queries that return information from this table.

For information on other tables in the advanced hunting schema, [see the advanced hunting reference](advanced-hunting-schema-tables.md).

| Column name | Data type | Description |
|-------------|-----------|-------------|
| `Timestamp` | datetime | Date and time when the event was recorded |
| `ActionType` | string | Type of activity that triggered the event |
| `Application` | string | Application that performed the recorded action |
| `FileName` | string | Name of the file that the recorded action was applied to |
| `FolderPath` | string | Folder containing the file that the recorded action was applied to |
| `PreviousFileName` | string | Original name of the file that was renamed as a result of the action |
| `AccountName` | string | User name of the account |
| `AccountDomain` | string | Domain of the account |
| `AccountUpn` | string | User principal name (UPN) of the account |
| `AccountObjectId` | string | Unique identifier for the account in Azure AD |
| `AccountDisplayName` | string | Name of the account user displayed in the address book. Typically a combination of a given or first name, a middle initiation, and a last name or surname. |
| `IPAddress` | string | IP address assigned to the endpoint and used during related network communications |
| `Location` | string | City, country, or other geographic location associated with the event |

## Related topics
- [Proactively hunt for threats](advanced-hunting-overview.md)
- [Learn the query language](advanced-hunting-query-language.md)
- [Use shared queries](advanced-hunting-shared-queries.md)
- [Hunt for threats across devices and emails](advanced-hunting-query-emails-devices.md)
- [Understand the schema](advanced-hunting-schema-tables.md)
- [Apply query best practices](advanced-hunting-best-practices.md)
