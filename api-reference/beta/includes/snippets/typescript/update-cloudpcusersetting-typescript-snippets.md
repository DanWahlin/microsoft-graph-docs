---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new CloudPcUserSetting()
requestBody.displayName = "Example";
requestBody.selfServiceEnabled = true;
requestBody.restorePointSetting = new CloudPcRestorePointSetting();
requestBody.restorePointSetting.frequencyInHours = "16";
requestBody.restorePointSetting.userRestoreEnabled = true;
requestBody.localAdminEnabled = false;
requestBody.additionalData = new Map<string, unknown>([
		["@odata.type", "#microsoft.graph.cloudPcUserSetting"]
	]);
async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.userSettingsById("cloudPcUserSetting-id").patch(requestBody);
}


```