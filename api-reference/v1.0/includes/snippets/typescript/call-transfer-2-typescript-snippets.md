---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.transferTarget = new InvitationParticipantInfo();
requestBody.transferTarget.identity = new IdentitySet();
requestBody.transferTarget.identity.user = new Identity();
requestBody.transferTarget.identity.user.id = "550fae72-d251-43ec-868c-373732c2704f";
requestBody.transferTarget.identity.user.displayName = "Heidi Steen";
requestBody.transferTarget.identity.user.additionalData = new Map<string, unknown>([
					["@odata.type", "#microsoft.graph.identity"]
				]);
requestBody.transferTarget.identity.additionalData = new Map<string, unknown>([
				["@odata.type", "#microsoft.graph.identitySet"]
			]);
requestBody.transferTarget.replacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d";
requestBody.transferTarget.additionalData = new Map<string, unknown>([
			["@odata.type", "#microsoft.graph.invitationParticipantInfo"],
			["endpointType", "default"]
		]);
async () => {
	await graphServiceClient.communications.callsById("call-id").transfer.post(requestBody);
}


```