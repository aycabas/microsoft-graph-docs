---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)


result, err := graphClient.ChatsById("chat-id").MessagesById("chatMessage-id").HostedContentsById("chatMessageHostedContent-id").Get()


```