---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new MobilityManagementPolicy()
requestBody.complianceUrl = "https://portal.mg.contoso.com/?portalAction=Compliance";
requestBody.discoveryUrl = "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc";
requestBody.termsOfUseUrl = "https://portal.mg.contoso.com/TermsofUse.aspx";
requestBody.additionalData = new Map<string, unknown>([
		["@odata.type", "#microsoft.graph.mobilityManagementPolicy"]
	]);
async () => {
	await graphServiceClient.policies.mobileAppManagementPoliciesById("mobilityManagementPolicy-id").patch(requestBody);
}


```