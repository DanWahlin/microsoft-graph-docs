---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new NamedLocation()
requestBody.displayName = "Updated named location without unknown countries and regions";
requestBody.additionalData = new Map<string, unknown>([
		["@odata.type", "#microsoft.graph.countryNamedLocation"],
		["countriesAndRegions", [
				"CA",
				"IN"
			]
		["includeUnknownCountriesAndRegions", false]
	]);
async () => {
	await graphServiceClient.identity.conditionalAccess.namedLocationsById("namedLocation-id").patch(requestBody);
}


```