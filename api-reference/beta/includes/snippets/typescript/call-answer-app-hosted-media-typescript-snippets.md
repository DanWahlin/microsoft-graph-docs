---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.callbackUri = "https://bot.contoso.com/api/calls";
requestBody.acceptedModalities = [
			"audio"
		]
requestBody.mediaConfig = new MediaConfig();
requestBody.mediaConfig.additionalData = new Map<string, unknown>([
			["@odata.type", "#microsoft.graph.appHostedMediaConfig"],
			["blob", "<Media Session Configuration Blob>"]
		]);
async () => {
	await graphServiceClient.communications.callsById("call-id").answer.post(requestBody);
}


```