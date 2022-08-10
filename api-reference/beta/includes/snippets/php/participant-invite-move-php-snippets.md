---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new InvitePostRequestBody();
$participantsInvitationParticipantInfo1 = new InvitationParticipantInfo();
$additionalData = [
'@odata.type' => '#microsoft.graph.invitationParticipantInfo', 
'replacesCallId' => 'a7ebfb2d-871e-419c-87af-27290b22e8db', 
'participantId' => '7d501bf1-5ee4-4605-ba92-0ae4513c611c', 
'identity' => $participantsInvitationParticipantInfo1 = new Identity();
$		participantsInvitationParticipantInfo1->set@odatatype('#microsoft.graph.identitySet');

$user = new User();
$		user->set@odatatype('#microsoft.graph.identity');

$		user->setId('682b6c37-0729-4fab-ace6-d730d5d9137e');

$		user->setIdentityProvider('AAD');


$participantsInvitationParticipantInfo1->setUser($user);

$participantsInvitationParticipantInfo1->setIdentity($identity);

];
$participantsInvitationParticipantInfo1->setAdditionalData($additionalData);



$participantsArray []= $participantsInvitationParticipantInfo1;
$requestBody->setParticipants($participantsArray);


$requestBody->setClientContext('f2fa86af-3c51-4bc2-8fc0-475452d9764f');



$requestResult = $graphServiceClient->communications()->callsById('call-id')->participants()->invite()->post($requestBody);


```