---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new AccessPackageCatalog()
requestBody.displayName = "Catalog One";
async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.catalogsById("accessPackageCatalog-id").patch(requestBody);
}


```