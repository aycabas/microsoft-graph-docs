---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
	"ConsistencyLevel": "eventual",
}

requestFilter := "startswith(displayName,%20'a')"
requestCount := true
requestTop := int32(1)

requestParameters := &graphconfig.ApplicationsRequestBuilderGetQueryParameters{
	Filter: &requestFilter,
	Count: &requestCount,
	Top: &requestTop,
	Orderby: [] string {"displayName"},
}
configuration := &graphconfig.ApplicationsRequestBuilderGetRequestConfiguration{
	Headers: headers,
	QueryParameters: requestParameters,
}

result, err := graphClient.Applications().GetWithRequestConfigurationAndResponseHandler(configuration, nil)


```