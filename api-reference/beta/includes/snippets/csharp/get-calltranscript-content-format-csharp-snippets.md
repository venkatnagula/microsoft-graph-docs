---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Users["{user-id}"].OnlineMeetings["{onlineMeeting-id}"].Transcripts["{callTranscript-id}"].Content
	.Request()
	.GetAsync();

```