---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new TokenIssuancePolicy()
requestBody.definition = [
			"definition-value"
		]
requestBody.displayName = "displayName-value";
requestBody.isOrganizationDefault = true;
async () => {
	await graphServiceClient.policies.tokenIssuancePoliciesById("tokenIssuancePolicy-id").patch(requestBody);
}


```