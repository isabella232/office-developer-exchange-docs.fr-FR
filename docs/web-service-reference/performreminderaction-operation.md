---
title: Opération PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Trouvez des informations sur l’opération EWS PerformReminderAction.
ms.openlocfilehash: 4c069d541e9a42167c447a50c405399958d3608d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462289"
---
# <a name="performreminderaction-operation"></a>Opération PerformReminderAction

Trouvez des informations sur l’opération EWS **PerformReminderAction** . 
  
L’opération **PerformReminderAction** les services Web Exchange (EWS) lance une action de rejet ou d’exécution répétée sur un rappel. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-performreminderaction-operation"></a>Utilisation de l’opération PerformReminderAction

Vous pouvez utiliser l’opération **PerformReminderAction** pour ignorer ou répéter les rappels renvoyés par l’opération [GetReminders](getreminders-operation.md) . Pour répéter un rappel, définissez le [ActionType](actiontype-reminderactiontype.md) sur **SNOOZE**et définissez la valeur [NewReminderTime](newremindertime.md) à une heure ultérieure à la [ReminderTime](remindertime.md)actuelle, sinon le **NewReminderTime** est ignoré par le serveur. Si le rappel est destiné à une occurrence d’une réunion périodique et que l’action de **répétition** est effectuée sur le rappel avec un **NewReminderTime** qui se trouve au-delà du rappel de l’occurrence suivante, le rappel est effectivement ignoré. 
  
Pour faire disparaître un rappel, définissez le paramètre **ActionType** sur **faire disparaître**. Lorsque le serveur traite la demande, le serveur remplace la valeur [IsReminderSet](isreminderset.md) de l’élément **true** par **false**.
  
### <a name="performreminderaction-operation-soap-headers"></a>En-têtes SOAP d’opération PerformReminderAction

L’opération **PerformReminderAction** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente. Cet en-tête s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a>Exemple de requête d’opération PerformReminderAction

L’exemple suivant de demande d’opération **PerformReminderAction** indique comment répéter un rappel actif et définir une nouvelle heure de rappel. Notez que vous devez inclure le **ChangeKey** pour l' [ItemId](itemid.md) et que le **NewReminderTime** doit être défini à une heure ultérieure à la **ReminderTime** renvoyée par l’opération [GetReminders](getreminders-operation.md) . 
  
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
    <m:PerformReminderAction>
      <m:ReminderItemActions>
        <t:ReminderItemAction>
          <t:ActionType>Snooze</t:ActionType>
          <t:ItemId Id="vwAAAA=="
           ChangeKey="DwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAUDA=="/>
          <t:NewReminderTime>2014-04-16T17:00:00Z</t:NewReminderTime>
        </t:ReminderItemAction>
      </m:ReminderItemActions>
    </m:PerformReminderAction>
  </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> La valeur **ItemId** a été raccourcie afin de préserver la lisibilité. 
  
Le corps SOAP de la demande contient les éléments suivants :
  
- [PerformReminderAction](performreminderaction.md)
    
- [ReminderItemActions](reminderitemactions.md)
    
- [ReminderItemAction](reminderitemaction.md)
    
- [ActionType](actiontype-reminderactiontype.md)
    
- [ItemId](itemid.md)
    
- [NewReminderTime](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a>Réponse de l’opération PerformReminderAction réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **PerformReminderAction** . L’élément **UpdatedItemIds** contient le **ItemIds** de l’élément de calendrier mis à jour. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

Le corps SOAP de réponse contient les éléments suivants :
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
- [ItemId](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a>Exemple de réponse d’erreur d’opération PerformReminderAction

L’exemple suivant montre une réponse à une demande d’opération **PerformReminderAction** lorsqu’aucune modification n’a été apportée sur le serveur. Il s’agit d’une réponse dans laquelle une demande a été envoyée, mais aucune **UpdatedItemIds** n’a été renvoyée, ce qui signifie qu’aucun rappel n’a été modifié. 
  
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
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

Le corps SOAP de la réponse d’erreur contient les éléments suivants :
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
Pour d’autres codes d’erreur qui sont génériques à EWS, consultez la rubrique [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi


- [Opération GetReminders](getreminders-operation.md)
    

