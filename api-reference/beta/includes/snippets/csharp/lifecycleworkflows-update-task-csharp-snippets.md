---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.IdentityGovernance.TaskObject
{
	Description = "Add user to selected groups",
	DisplayName = "Update marketing day 1 add users to Group set up",
};
var result = await graphClient.IdentityGovernance.LifecycleWorkflows.Workflows["{workflow-id}"].Tasks["{task-id}"].PatchAsync(requestBody);


```