---
title: Opération GetReminders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: Opération de recherche plus d’informations sur la GetReminders EWS.
ms.openlocfilehash: 803dabf51b94dbd8fb01f2709a42ff59a597bfd1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756727"
---
# <a name="getreminders-operation"></a>Opération GetReminders

Trouvez des informations sur l’opération EWS **GetReminders** . 
  
L’opération d’Exchange Web Services (EWS) **GetReminders** récupère les rappels pour les éléments de calendrier et des tâches. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getreminders-operation"></a>Utilisation de l’opération GetReminders

L’opération **GetReminders** Obtient les rappels pour actuel et futur de calendrier et les tâches dans la boîte aux lettres de l’utilisateur, selon les valeurs des éléments transmis dans la demande. L’opération peut récupérer tous les éléments de calendrier actuels et futurs ainsi que les tâches qui ont un rappel à définir. Éléments de calendrier privés sont inclus dans les réponses. Tâches sans rappels ne sont pas inclus dans les réponses, ni sont des messages électroniques avec des rappels ou les indicateurs de suivi. 
  
Pour récupérer tous les rappels actifs, nous vous recommandons de définir la [ReminderType](remindertype.md) pour **toutes les** et l' [heure de fin](endtime-remindermessagedatatype.md) à l’heure actuelle. 
  
Si les éléments [BeginTime](begintime.md) et **EndTime** sont inclus dans la demande, la réponse inclut des rappels pour n’importe quel calendrier et éléments de tâche qui se produisent entre possèdent un rappel qui se produit entre le **BeginTime** et de **fin**.
  
Le tableau suivant décrit le comportement de l’élément **ReminderType** lorsque les éléments **BeginTime** et **l’heure de fin** sont inclus. 
  
|** ReminderType élément valeur **|**Description**|
|:-----|:-----|
|Tous  <br/> |Rappels qui se produisent entre le **BeginTime** et de **fin**.  <br/> |
|En cours  <br/> |Rappels renvoyés par **tous les**, ainsi que les rappels qui sont antérieurs à la fenêtre de temps demandé, s’il est toujours en cours, ainsi que tous les rendez-vous, quel que soit l’âge.  <br/> |
|Ancienne  <br/> |Rappels retournées par **tous les**, moins les événements qui ne sont pas terminées, moins tous les rendez-vous. Les éléments **BeginTime** et **l’heure de fin** doivent être définies à utiliser **l’ancienne** valeur.  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>En-têtes SOAP GetReminders opération

L’opération **GetReminders** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Cet en-tête est applicable à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="getreminders-operation-request-example"></a>Exemple de requête d’opération GetReminders

Une demande d’opération **GetReminders** l’exemple suivant montre comment extraire les éléments de cinq calendrier premier qui se produisent entre le **BeginTime** et de **fin**.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetReminders>
      <m:EndTime>2014-04-16T21:00:00Z</m:EndTime>
      <m:ReminderType>All</m:ReminderType>
    </m:GetReminders>
  </soap:Body>
</soap:Envelope>
```

L’exemple de demande SOAP body contient les éléments suivants :
  
- [GetReminders](getreminders.md)
    
- [Heure de fin](endtime-remindermessagedatatype.md)
    
- [ReminderType](remindertype.md)
    
Le corps SOAP peut également contenir les éléments suivants :
  
- [BeginTime](begintime.md)
    
- [MaxItems](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>Réponse d’opération GetReminders réussie

L’exemple suivant montre une réponse positive à une demande d’opération **GetReminders** . La réponse contient un rappel pour l’élément de calendrier « Réunion d’équipe » et un rappel pour la tâche « Tâches pour envoyer des notes de réunion ». 
  
> [!NOTE]
> Les identificateurs ont été réduits afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Team meeting</Subject>
          <Location />
          <ReminderTime>2014-04-15T21:00:00Z</ReminderTime>
          <StartDate>2014-04-15T21:00:00Z</StartDate>
          <EndDate>2014-04-15T21:30:00Z</EndDate>
          <ItemId Id="vQAAAA=="
                  ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV4" />
          <RecurringMasterItemId Id="K7u5AAA=" ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV0" />
          <ReminderGroup>Calendar</ReminderGroup>
          <UID>6CF2FA62</UID>
        </Reminder>
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Task to send meeting notes</Subject>
          <Location />
          <ReminderTime>2014-04-16T14:00:00Z</ReminderTime>
          <StartDate>0001-01-02T00:00:00Z</StartDate>
          <EndDate>0001-01-02T00:00:00Z</EndDate>
          <ItemId Id="vAAAAA=="
                  ChangeKey="EwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAIDg==" />
          <ReminderGroup>Task</ReminderGroup>
          <UID>vAAAAA==</UID>
        </Reminder>
      </Reminders>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

La réponse SOAP body contient les éléments suivants :
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [Rappels](reminders.md)
    
- [Rappel](reminder.md)
    
- [Objet](subject.md)
    
- [Location](location-remindermessagedatatype.md)
    
- [ReminderTime](remindertime.md)
    
- [Date de début](startdate.md)
    
- [Date de fin](enddate-remindertype.md)
    
- [ID d’élément](itemid.md)
    
- [RecurringMasterItemId](recurringmasteritemid.md)
    
- [ReminderGroup](remindergroup.md)
    
- [UID](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a>Exemple de réponse d’erreur opération GetReminders

L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetReminders** . Il s’agit d’une réponse à une demande dans laquelle la date de fin est antérieure à la date de début. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi


- [PerformReminderAction](performreminderaction.md)
    

