---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new EducationAssignmentResource()
requestBody.distributeForStudentWork = false;
requestBody.resource = new EducationResource();
requestBody.resource.displayName = "Graph Doc pages.xlsx";
requestBody.resource.additionalData = new Map<string, unknown>([
			["@odata.type", "microsoft.graph.educationExcelResource"],
			["fileUrl", "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RIR7PSV4JJSFJHKNPUVUWGPW4O2"]
		]);
const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").resources.post(requestBody);
}


```