---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.securityEnabledOnly = true;
const result = async () => {
	await graphServiceClient.me.getMemberGroups.post(requestBody);
}


```