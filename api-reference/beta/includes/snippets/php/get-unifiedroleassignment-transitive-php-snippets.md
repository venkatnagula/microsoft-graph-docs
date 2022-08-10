---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestConfiguration = new TransitiveRoleAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new TransitiveRoleAssignmentsRequestBuilderGetQueryParameters();
$queryParameters->count = true;
$queryParameters->filter = "principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516' and roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'";

$headers = [
'ConsistencyLevel' => 'eventual',
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$requestResult = $graphServiceClient->roleManagement()->directory()->transitiveRoleAssignments()->get($requestConfiguration);


```