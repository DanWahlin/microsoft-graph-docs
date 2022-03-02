---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new User()
requestBody.customSecurityAttributes = new CustomSecurityAttributeValue();
requestBody.customSecurityAttributes.additionalData = new Map<string, unknown>([
				 ["@odata.type" , "#Microsoft.DirectoryServices.CustomSecurityAttributeValue"],
				 ["projectDate" , "2022-10-01"],
		]);
async () => {
	await graphServiceClient.usersById("user-id").patch(requestBody);
}


```