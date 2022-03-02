---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new DataSource()
requestBody.additionalData = new Map<string, unknown>([
		["@odata.type", "microsoft.graph.ediscovery.siteSource"],
			 ["webUrl" , "https://contoso.sharepoint.com/sites/SecretSite"],
	]);
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").sourceCollectionsById("sourceCollection-id").additionalSources.post(requestBody);
}


```