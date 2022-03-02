---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.topic = new TeamworkActivityTopic();
requestBody.topic.source = "entityUrl";
requestBody.topic.value = "https://graph.microsoft.com/v1.0/users/{userId}/teamwork/installedApps/{installationId}";
requestBody.activityType = "taskCreated";
requestBody.previewText = new ItemBody();
requestBody.previewText.content = "New Task Created";
const keyvaluepair = new KeyValuePair();
keyvaluepair.additionalData = new Map<string, unknown>([
					["name", "taskId"],
					["value", "Task 12322"]
				]);
requestBody.templateParameters = [
			keyvaluepair
		]
async () => {
	await graphServiceClient.usersById("user-id").teamwork.sendActivityNotification.post(requestBody);
}


```