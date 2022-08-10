---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewChatMessage()
messageType := graphmodels.MESSAGE_CHATMESSAGETYPE 
requestBody.SetMessageType(&messageType) 
subject := null
requestBody.SetSubject(&subject) 
summary := null
requestBody.SetSummary(&summary) 
importance := graphmodels.NORMAL_CHATMESSAGEIMPORTANCE 
requestBody.SetImportance(&importance) 
locale := "en-us"
requestBody.SetLocale(&locale) 
from := graphmodels.Newfrom()
application := null
from.SetApplication(&application) 
device := null
from.SetDevice(&device) 
user := graphmodels.NewIdentity()
id := "3b102402-813e-4e17-a6b2-f841aef1fdfc"
user.SetId(&id) 
displayName := "Sumit Gupta"
user.SetDisplayName(&displayName) 
additionalData := map[string]interface{}{
	"userIdentityType" : "aadUser", 
}
user.SetAdditionalData(additionalData)
from.SetUser(user)
additionalData := map[string]interface{}{
	conversation := null
from.SetConversation(&conversation) 
}
from.SetAdditionalData(additionalData)
requestBody.SetFrom(from)
body := graphmodels.NewItemBody()
contentType := graphmodels.TEXT_BODYTYPE 
body.SetContentType(&contentType) 
content := "Edit text only"
body.SetContent(&content) 
requestBody.SetBody(body)
attachments := []graphmodels.ChatMessageAttachmentable {

}
requestBody.SetAttachments(attachments)
mentions := []graphmodels.ChatMessageMentionable {

}
requestBody.SetMentions(mentions)
reactions := []graphmodels.ChatMessageReactionable {

}
requestBody.SetReactions(reactions)

graphClient.TeamsById("team-id").ChannelsById("channel-id").MessagesById("chatMessage-id").Patch(requestBody)


```