---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.userAccountType = "administrator";
requestBody.osVersion = "windows10";
async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.cloudPCsById("cloudPC-id").reprovision.post(requestBody);
}


```