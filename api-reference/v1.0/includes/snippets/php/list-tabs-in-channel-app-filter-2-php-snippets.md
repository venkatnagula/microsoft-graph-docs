---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestConfiguration = new TabsRequestBuilderGetRequestConfiguration();
$queryParameters = TabsRequestBuilderGetRequestConfiguration::createQueryParameters();
$queryParameters->expand = ["teamsApp"];
$queryParameters->filter = "teamsApp/id eq 'com.microsoft.teamspace.tab.planner'";
$requestConfiguration->queryParameters = $queryParameters;


$result = $graphServiceClient->teamsById('team-id')->channelsById('channel-id')->tabs()->get($requestConfiguration);


```