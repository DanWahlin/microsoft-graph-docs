---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new User()
requestBody.passwordProfile = new PasswordProfile();
requestBody.passwordProfile.forceChangePasswordNextSignIn = false;
requestBody.passwordProfile.password = "xWwvJ]6NMw+bWH-d";
async () => {
	await graphServiceClient.usersById("user-id").patch(requestBody);
}


```