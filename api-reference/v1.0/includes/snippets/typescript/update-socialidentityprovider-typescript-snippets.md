---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new IdentityProviderBase()
requestBody.additionalData = new Map<string, unknown>([
		["@odata.type", "#microsoft.graph.socialIdentityProvider"],
		["clientSecret", "1111111111111"]
	]);
async () => {
	await graphServiceClient.identity.identityProvidersById("identityProviderBase-id").patch(requestBody);
}


```