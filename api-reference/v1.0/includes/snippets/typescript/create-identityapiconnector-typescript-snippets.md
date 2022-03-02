---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new IdentityApiConnector()
requestBody.displayName = "Test API";
requestBody.targetUrl = "https://someotherapi.com/api";
requestBody.authenticationConfiguration = new ApiAuthenticationConfigurationBase();
requestBody.authenticationConfiguration.additionalData = new Map<string, unknown>([
			["@odata.type", "#microsoft.graph.pkcs12Certificate"],
			["pkcs12Value", "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA"],
			["password", "CertificatePassword"]
		]);
const result = async () => {
	await graphServiceClient.identity.apiConnectors.post(requestBody);
}


```