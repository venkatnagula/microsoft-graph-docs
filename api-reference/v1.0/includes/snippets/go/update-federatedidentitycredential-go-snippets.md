---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewFederatedIdentityCredential()
name := "testing02"
requestBody.SetName(&name) 
issuer := "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0"
requestBody.SetIssuer(&issuer) 
subject := "a7d388c3-5e3f-4959-ac7d-786b3383006a"
requestBody.SetSubject(&subject) 
description := "Updated description"
requestBody.SetDescription(&description) 
audiences := []string {
	"api://AzureADTokenExchange",

}
requestBody.SetAudiences(audiences)

graphClient.ApplicationsById("application-id").FederatedIdentityCredentialsById("federatedIdentityCredential-id").Patch(requestBody)


```