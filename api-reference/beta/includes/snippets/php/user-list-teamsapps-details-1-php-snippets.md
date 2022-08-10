---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestConfiguration = new UserScopeTeamsAppInstallationRequestBuilderGetRequestConfiguration();

$queryParameters = new UserScopeTeamsAppInstallationRequestBuilderGetQueryParameters();
$queryParameters->expand = ["teamsAppDefinition"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->usersById('user-id')->teamwork()->installedAppsById('userScopeTeamsAppInstallation-id')->get($requestConfiguration);


```