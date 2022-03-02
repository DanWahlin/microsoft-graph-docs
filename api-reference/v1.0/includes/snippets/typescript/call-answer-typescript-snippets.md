---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.callbackUri = "callbackUri-value";
requestBody.mediaConfig = new MediaConfig();
requestBody.mediaConfig.additionalData = new Map<string, unknown>([
			["@odata.type", "#microsoft.graph.appHostedMediaConfig"],
			["blob", "<Media Session Configuration Blob>"]
		]);
requestBody.acceptedModalities = [
			"audio"
		]
requestBody.participantCapacity = 200;
async () => {
	await graphServiceClient.communications.callsById("call-id").answer.post(requestBody);
}


```