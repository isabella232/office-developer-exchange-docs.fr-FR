---
title: Opération GetReminders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: Trouvez des informations sur l’opération EWS GetReminders.
ms.openlocfilehash: dcbe20c674d7524a7776d374fa6964899abf472f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458305"
---
# <a name="getreminders-operation"></a>Opération GetReminders

Trouvez des informations sur l’opération EWS **GetReminders** . 
  
L’opération **GetReminders** les services Web Exchange (EWS) récupère les rappels pour les éléments de calendrier et de tâche. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getreminders-operation"></a>Utilisation de l’opération GetReminders

L’opération **GetReminders** obtient des rappels pour les éléments de calendrier et de tâche actuels et futurs dans la boîte aux lettres de l’utilisateur, en fonction des valeurs d’élément transmises dans la demande. L’opération peut récupérer tous les éléments de calendrier actuels et futurs, ainsi que les tâches qui ont un rappel défini. Les éléments de calendrier privés sont inclus dans les réponses. Les tâches sans rappel ne sont pas incluses dans les réponses, ni dans les messages avec des rappels ou avec des indicateurs de suivi. 
  
Pour récupérer tous les rappels en cours, nous vous recommandons de définir [ReminderType](remindertype.md) sur **All** [et l’heure](endtime-remindermessagedatatype.md) de fin sur l’heure actuelle. 
  
Si les éléments [BeginTime](begintime.md) et **EndTime** sont inclus dans la demande, la réponse inclut des rappels pour tous les éléments de calendrier et de tâche qui se produisent entre les ont un rappel qui se produit entre **BeginTime** et **EndTime**.
  
Le tableau suivant décrit le comportement de l’élément **ReminderType** lorsque les éléments **BeginTime** et **EndTime** sont inclus. 
  
|ReminderType * * valeur de l’élément * *|**Description**|
|:-----|:-----|
|Tous  <br/> |Rappels qui se produisent entre **BeginTime** et **EndTime**.  <br/> |
|Current  <br/> |Rappels retournés par **tous**, plus rappels qui sont antérieurs à la fenêtre de temps demandée si l’événement est encore en cours, plus tous les rendez-vous, quel que soit leur âge.  <br/> |
|Ancien  <br/> |Rappels renvoyés par **tous les**, moins les événements qui n’ont pas encore été terminés, moins tous les rendez-vous. Les éléments **BeginTime** et **EndTime** doivent être définis pour utiliser l' **ancienne** valeur.  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>En-têtes SOAP d’opération GetReminders

L’opération **GetReminders** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente. Cet en-tête s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getreminders-operation-request-example"></a>Exemple de requête d’opération GetReminders

L’exemple suivant de demande d’opération **GetReminders** indique comment récupérer les cinq premiers éléments de calendrier qui se produisent entre **BeginTime** et **EndTime**.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

Le corps SOAP de requête de l’exemple contient les éléments suivants :
  
- [GetReminders](getreminders.md)
    
- [EndTime](endtime-remindermessagedatatype.md)
    
- [ReminderType](remindertype.md)
    
Le corps SOAP peut également contenir les éléments suivants :
  
- [BeginTime](begintime.md)
    
- [MaxItems](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>Réponse de l’opération GetReminders réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **GetReminders** . La réponse contient un rappel pour l’élément de calendrier « réunion d’équipe » et un rappel pour la tâche « tâche d’envoi de notes de réunion ». 
  
> [!NOTE]
> Les identificateurs ont été raccourcis pour conserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
        <Reminder xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

Le corps SOAP de réponse contient les éléments suivants :
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [Reminders](reminders.md)
    
- [Reminder](reminder.md)
    
- [Subject](subject.md)
    
- [Emplacement](location-remindermessagedatatype.md)
    
- [ReminderTime](remindertime.md)
    
- [StartDate](startdate.md)
    
- [EndDate](enddate-remindertype.md)
    
- [ItemId](itemid.md)
    
- [RecurringMasterItemId](recurringmasteritemid.md)
    
- [ReminderGroup](remindergroup.md)
    
- [UID](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a>Exemple de réponse d’erreur d’opération GetReminders

L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetReminders** . Il s’agit d’une réponse à une demande dans laquelle la date de fin était antérieure à la date de début. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

Le corps SOAP de la réponse d’erreur contient les éléments suivants :
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi


- [PerformReminderAction](performreminderaction.md)
    

