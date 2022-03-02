---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.additionalData = new Map<string, unknown>([
		["@odata.id", "https://graph.microsoft.com/beta/identity/identityProviders/{id}"],
		["@odata.type", "#microsoft.graph.identityProvider"]
	]);
async () => {
	await graphServiceClient.identity.b2cUserFlowsById("b2cIdentityUserFlow-id").userFlowIdentityProviders.$ref.patch(requestBody);
}


```