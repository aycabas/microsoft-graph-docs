---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)


requestToken := "1230919asd190410jlka"

requestParameters := &graphconfig.DeltaRequestBuilderGetQueryParameters{
	Token: &requestToken,
}
configuration := &graphconfig.DeltaRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.SitesById("site-id").ListsById("list-id").Items().Delta().GetWithRequestConfigurationAndResponseHandler(configuration, nil)


```