# GitSync

## Connectors
|Name|Description|Has Mappings|
|----|-----------|------------|
|Google Chronicle - Chronicle Alerts Connector 1|Pull information about Rule based alerts from Google Chronicle. Note: dynamic list is used for filtering purposes. For all of the details please visit the documentation portal.|False|
|Sample Integration - Simple Connector Example|This is an example of a simple connector. It's integrated with "api.vatcomply.com" service and provides all of the main design ideas necessary to build a stable connector. Dynamic List defines what rates should be returned for a given currency and expects input in the format "EUR" etc.|False|


## Visual Families
|Name|Description|
|----|-----------|
|Copy of AV|Anti-virus alerts visualization|
|Playground_Upgraded_Legacy_Visual_Families_1|Playground_Upgraded_Legacy_Visual_Families_1|
|Playground_Upgraded_Legacy_Visual_Families_2|Playground_Upgraded_Legacy_Visual_Families_2|


## Jobs
|Name|Description|
|----|-----------|
|Google Chronicle Alerts Creator Job|This job will sync new SOAR alerts with Chronicle SIEM.Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.|
|Google Chronicle Sync Job|This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM. Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.|
|Refresh Token Renewal Job|Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.|
|Sync Incidents|This job synchronizes Google SecOps Alerts and Microsoft Sentinel Incidents. It ensures that comments, status, and tags are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the “Microsoft Sentinel Incident” tag. If the alert didn’t originate from “Microsoft Azure Sentinel Incident Connector v2”,  you will need to add an “Incident_ID” context value to the case for the job to be able to find the correct information.|

