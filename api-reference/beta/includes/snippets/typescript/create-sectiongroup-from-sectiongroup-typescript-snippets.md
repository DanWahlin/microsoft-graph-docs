---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.additionalData = new Map<string, unknown>([
		["displayName", "Section group name"]
	]);
async () => {
	await graphServiceClient.me.onenote.sectionGroupsById("sectionGroup-id").sectionGroups.post(requestBody);
}


```