---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ListItem()
requestBody.fields = new FieldValueSet();
requestBody.fields.additionalData = new Map<string, unknown>([
			["Title", "Widget"],
			["Color", "Purple"],
			["Weight", 32]
		]);
const result = async () => {
	await graphServiceClient.sitesById("site-id").listsById("list-id").items.post(requestBody);
}


```