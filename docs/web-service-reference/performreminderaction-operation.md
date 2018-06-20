---
title: Opération PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Opération de recherche plus d’informations sur la PerformReminderAction EWS.
ms.openlocfilehash: 778fbb508413721f58cfcf9143a5296874e6cd1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828722"
---
# <a name="performreminderaction-operation"></a>Opération PerformReminderAction

Trouvez des informations sur l’opération EWS **PerformReminderAction** . 
  
L’opération d’Exchange Web Services (EWS) **PerformReminderAction** lance une action d’ignorer ou répéter un rappel. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-performreminderaction-operation"></a>Utilisation de l’opération PerformReminderAction

Vous pouvez utiliser l’opération **PerformReminderAction** pour fermer ou de répéter rappels (retard) retournées par l’opération [GetReminders](getreminders-operation.md) . Pour répéter un rappel, définir l' [ActionType](actiontype-reminderactiontype.md) **répétés**et définir la valeur de [NewReminderTime](newremindertime.md) à une date postérieure à la actuel [ReminderTime](remindertime.md), sinon la **NewReminderTime** est ignoré par le serveur. Si le rappel est une occurrence d’une réunion périodique, et l’action **Snooze** est exécutée sur le rappel avec un **NewReminderTime** qui a passé le rappel de la prochaine occurrence, le rappel est rejeté efficacement. 
  
Pour faire disparaître un rappel, définissez l' **ActionType** pour **faire disparaître**. Lorsque le serveur traite la demande, le serveur modifie la valeur de [IsReminderSet](isreminderset.md) pour l’élément de **la valeur True** à **False**.
  
### <a name="performreminderaction-operation-soap-headers"></a>En-têtes SOAP PerformReminderAction opération

L’opération **PerformReminderAction** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Cet en-tête est applicable à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a>Exemple de requête d’opération PerformReminderAction

Une demande d’opération **PerformReminderAction** l’exemple suivant montre comment répéter un rappel en cours et définir une nouvelle heure du rappel. Notez que vous devez inclure le **ChangeKey** pour l' [ID d’élément](itemid.md) et le **NewReminderTime** doit être définie à une date postérieure à la **ReminderTime** retournées par l’opération [GetReminders](getreminders-operation.md) . 
  
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
  
La demande SOAP body contient les éléments suivants :
  
- [PerformReminderAction](performreminderaction.md)
    
- [ReminderItemActions](reminderitemactions.md)
    
- [ReminderItemAction](reminderitemaction.md)
    
- [ActionType](actiontype-reminderactiontype.md)
    
- [ID d’élément](itemid.md)
    
- [NewReminderTime](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a>Réponse d’opération PerformReminderAction réussie

L’exemple suivant montre une réponse positive à une demande d’opération **PerformReminderAction** . L’élément **UpdatedItemIds** contient les **numéros d’objet** de l’élément de calendrier mis à jour. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

La réponse SOAP body contient les éléments suivants :
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
- [ID d’élément](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a>Exemple de réponse d’erreur opération PerformReminderAction

L’exemple suivant montre une réponse à une demande d’opération **PerformReminderAction** lorsqu’aucune modification n’a été effectuée sur le serveur. Il s’agit d’une réponse dans lequel une demande a été envoyée, mais aucun **UpdatedItemIds** ont été retournés, ce qui signifie aucune rappels ont été modifiées. 
  
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
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
Pour les codes d’erreur supplémentaires qui sont génériques pour EWS, voir [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi


- [Opération GetReminders](getreminders-operation.md)
    

