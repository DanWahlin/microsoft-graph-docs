---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new Attachment()
requestBody.name = "Personal pictures";
requestBody.additionalData = new Map<string, unknown>([
		["@odata.type", "#microsoft.graph.referenceAttachment"],
		["sourceUrl", "https://contoso.com/personal/mario_contoso_net/Documents/Pics"],
		["providerType", "oneDriveConsumer"],
		["permission", "Edit"],
		["isFolder", "True"]
	]);
const result = async () => {
	await graphServiceClient.me.messagesById("message-id").attachments.post(requestBody);
}


```