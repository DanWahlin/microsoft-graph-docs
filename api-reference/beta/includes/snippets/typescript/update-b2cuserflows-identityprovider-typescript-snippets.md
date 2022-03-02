---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.additionalData = new Map<string, unknown>([
		["@odata.id", "https://graph.microsoft.com/beta/identityProviders/{id}"]
	]);
const result = async () => {
	await graphServiceClient.identity.b2cUserFlowsById("b2cIdentityUserFlow-id").identityProviders.$ref.post(requestBody);
}


```