---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new B2cIdentityUserFlow()
requestBody.id = "UserFlowWithAPIConnector";
requestBody.userFlowType = "signUpOrSignIn";
requestBody.userFlowTypeVersion = 1;
requestBody.apiConnectorConfiguration = new UserFlowApiConnectorConfiguration();
requestBody.apiConnectorConfiguration.postFederationSignup = new IdentityApiConnector();
requestBody.apiConnectorConfiguration.postFederationSignup.additionalData = new Map<string, unknown>([
				["@odata.id", "{apiConnectorId}"]
			]);
requestBody.apiConnectorConfiguration.postAttributeCollection = new IdentityApiConnector();
requestBody.apiConnectorConfiguration.postAttributeCollection.additionalData = new Map<string, unknown>([
				["@odata.id", "{apiConnectorId}"]
			]);
const result = async () => {
	await graphServiceClient.identity.b2cUserFlows.post(requestBody);
}


```