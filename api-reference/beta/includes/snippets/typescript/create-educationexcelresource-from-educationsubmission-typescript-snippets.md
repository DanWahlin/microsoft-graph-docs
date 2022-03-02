---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new EducationSubmissionResource()
requestBody.resource = new EducationResource();
requestBody.resource.displayName = "userAgeGroup QueryParameter Test.xlsx";
requestBody.resource.additionalData = new Map<string, unknown>([
			["@odata.type", "#microsoft.graph.educationExcelResource"],
			["fileUrl", "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RONPUDM2CZKNRF3TGHYUM7Z64WE"]
		]);
const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").submissionsById("educationSubmission-id").resources.post(requestBody);
}


```