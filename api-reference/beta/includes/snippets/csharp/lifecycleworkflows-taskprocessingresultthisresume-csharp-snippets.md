---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.IdentityGovernance.LifecycleWorkflows.Workflows.Item.Tasks.Item.TaskProcessingResults.Item.MicrosoftGraphIdentityGovernanceResume.ResumePostRequestBody
{
	Data = new Microsoft.Graph.Beta.Models.IdentityGovernance.CustomTaskExtensionCallbackData
	{
		OperationStatus = Microsoft.Graph.Beta.Models.IdentityGovernance.CustomTaskExtensionOperationStatus.Completed,
	},
	Source = "sample",
	Type = "lifecycleEvent",
};
await graphClient.IdentityGovernance.LifecycleWorkflows.Workflows["{workflow-id}"].Tasks["{task-id}"].TaskProcessingResults["{taskProcessingResult-id}"].MicrosoftGraphIdentityGovernanceResume.PostAsync(requestBody);


```