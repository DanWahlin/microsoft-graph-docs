---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.additionalData = new Map<string, unknown>([
		["@odata.id", "https://graph.microsoft.com/beta/groups/{id}"]
	]);
const result = async () => {
	await graphServiceClient.print.sharesById("printerShare-id").allowedGroups.$ref.post(requestBody);
}


```