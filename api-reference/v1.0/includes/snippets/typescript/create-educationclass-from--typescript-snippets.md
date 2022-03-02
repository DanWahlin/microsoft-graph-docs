---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new EducationClass()
requestBody.displayName = "String";
requestBody.mailNickname = "String";
requestBody.description = "String";
requestBody.createdBy = new IdentitySet();
requestBody.createdBy.additionalData = new Map<string, unknown>([
			["@odata.type", "microsoft.graph.identitySet"]
		]);
requestBody.classCode = "String";
requestBody.externalName = "String";
requestBody.externalId = "String";
requestBody.externalSource = "String";
requestBody.externalSourceDetail = "String";
requestBody.grade = "String";
requestBody.term = new EducationTerm();
requestBody.term.additionalData = new Map<string, unknown>([
			["@odata.type", "microsoft.graph.educationTerm"]
		]);
requestBody.additionalData = new Map<string, unknown>([
		["@odata.type", "#microsoft.graph.educationClass"]
	]);
const result = async () => {
	await graphServiceClient.education.classes.post(requestBody);
}


```