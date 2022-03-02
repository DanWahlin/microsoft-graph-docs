---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ConversationMember()
requestBody.roles = [
			"owner"
		]
requestBody.additionalData = new Map<string, unknown>([
		["@odata.type", "#microsoft.graph.aadUserConversationMember"],
		["user@odata.bind", "https://graph.microsoft.com/beta/users('jacob@contoso.com')"]
	]);
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").members.post(requestBody);
}


```