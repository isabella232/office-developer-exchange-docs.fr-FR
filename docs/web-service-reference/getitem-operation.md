---
title: Opération GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Trouvez des informations sur l’opération EWS de GetItem.
localization_priority: Priority
ms.openlocfilehash: 8871dde183974454fc27dbddda489e6b0a70f3aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463327"
---
# <a name="getitem-operation"></a>Opération GetItem

Trouvez des informations sur l’opération EWS de **GetItem** . 
  
L’opération **GetItem** obtient des éléments de la Banque d’Exchange. 
  
## <a name="using-the-getitem-operation"></a>Utilisation de l’opération GetItem

L’opération **GetItem** renvoie de nombreuses propriétés d’élément. Les propriétés renvoyées dans une réponse **GetItem** varient en fonction de la forme demandée, des propriétés supplémentaires demandées et du type d’élément renvoyé. 
  
Les éléments de [message](message-ex15websvcsotherref.md) représentent les messages électroniques et tous les autres éléments qui ne sont pas fortement typés par le schéma des services Web Exchange (EWS). Des éléments tels que IPM. Le partage et IPM. InfoPath sont renvoyés en tant qu’éléments [message](message-ex15websvcsotherref.md) . Exchange ne retourne pas l’élément [élément](item.md) de base dans les réponses. 
  
L’opération **GetItem** ne retourne pas les pièces jointes. Elle renvoie les métadonnées d’un élément ou d’un fichier attaché. Pour renvoyer une pièce jointe, utilisez l' [opération GetAttachment](getattachment-operation.md).
  
## <a name="getitem-operation-soap-headers"></a>En-têtes SOAP d’opération GetItem

L’opération **GetItem** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|En-tête * * * *|****Element****|****Description****|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |Spécifie la résolution des valeurs de données/temps dans les réponses du serveur, soit en secondes, soit en millisecondes.  <br/> |
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifie le fuseau horaire à utiliser pour toutes les réponses du serveur.  <br/> |
   
## <a name="in-this-section"></a>Dans cette section

[Opération GetItem (message électronique)](getitem-operation-email-message.md)
  
[Opération de GetItem (élément de calendrier)](getitem-operation-calendar-item.md)
  
[Opération GetItem (tâche)](getitem-operation-task.md)
  
[Opération GetItem (contact)](getitem-operation-contact.md)
  
## <a name="see-also"></a>Voir aussi



[Référence EWS pour Exchange](ews-reference-for-exchange.md)

