---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new B2cIdentityUserFlow();
$requestBody->setIsLanguageCustomizationEnabled(true);

$requestBody->setDefaultLanguageTag('en');



$graphServiceClient->identity()->b2cUserFlowsById('b2cIdentityUserFlow-id')->patch($requestBody);


```