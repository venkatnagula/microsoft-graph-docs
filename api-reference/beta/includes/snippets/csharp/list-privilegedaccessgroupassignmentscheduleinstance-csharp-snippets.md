---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.IdentityGovernance.PrivilegedAccess.Group.AssignmentScheduleInstances.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "groupId eq '2b5ed229-4072-478d-9504-a047ebd4b07d'";
});


```