---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new PlannerUser()
requestBody.favoritePlanReferences = new PlannerFavoritePlanReferenceCollection();
requestBody.favoritePlanReferences.additionalData = new Map<string, unknown>([
				 ["@odata.type" , "#microsoft.graph.plannerFavoritePlanReference"],
				 ["orderHint" , " !"],
				 ["planTitle" , "Next Release Discussion"],
			["7oTB5aMIAE2rVo-1N-L7RmQAGX2q", null],
		]);
requestBody.recentPlanReferences = new PlannerRecentPlanReferenceCollection();
requestBody.recentPlanReferences.additionalData = new Map<string, unknown>([
				 ["@odata.type" , "#microsoft.graph.plannerRecentPlanReference"],
				 ["lastAccessedDateTime" , "2018-01-02T22:49:46.155Z"],
				 ["planTitle" , "Next Release Discussion"],
		]);
const headers = {
	"Prefer": "return=representation",
	"If-Match": "W/\"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc=\"",
};
async () => {
	await graphServiceClient.me.planner.patch(requestBody, headers);
}


```