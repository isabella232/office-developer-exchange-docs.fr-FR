---
title: GetItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Pour des informations sur la EWS GetItem operation.
ms.openlocfilehash: 9b63032b2eaa3bf26027a42e38bfa06bedcbac86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756660"
---
# <a name="getitem-operation"></a>GetItem Operation

Trouvez des informations sur l’opération EWS **GetItem** . 
  
L’opération **GetItem** Obtient les éléments à partir de la banque d’informations Exchange. 
  
## <a name="using-the-getitem-operation"></a>Utilisation de l’opération GetItem

L’opération **GetItem** renvoie plusieurs propriétés de l’élément. Les propriétés qui sont retournées dans une réponse **GetItem** varient en fonction de la forme demandée, des propriétés supplémentaires requises et le type d’élément renvoyé. 
  
Éléments de [message](message-ex15websvcsotherref.md) représentent des messages électroniques et tous les autres éléments qui ne sont pas fortement typées dans le schéma Exchange Web Services (EWS). Éléments tels que IPM. Partage et IPM.InfoPath sont renvoyés en tant qu’éléments du [Message](message-ex15websvcsotherref.md) . Exchange ne renvoie pas de [l’élément de base](item.md) des réponses. 
  
L’opération **GetItem** ne renvoie pas les pièces jointes. Il retourne les métadonnées relatives à un fichier ou un élément attaché. Pour renvoyer une pièce jointe, utilisez l' [opération GetAttachment](getattachment-operation.md).
  
## <a name="getitem-operation-soap-headers"></a>En-têtes SOAP GetItem opération

L’opération de **GetItem** peut utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|En-tête ***|****Element****|****Description****|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |Spécifie la résolution des valeurs de date/heure dans les réponses à partir du serveur, en secondes ou en millisecondes.  <br/> |
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifie le fuseau horaire à utiliser pour toutes les réponses à partir du serveur.  <br/> |
   
## <a name="in-this-section"></a>Contenu de cette section

[Opération de GetItem (e-mail)](getitem-operation-email-message.md)
  
[Opération de GetItem (élément de calendrier)](getitem-operation-calendar-item.md)
  
[Opération de GetItem (tâche)](getitem-operation-task.md)
  
[Opération de GetItem (contacts)](getitem-operation-contact.md)
  
## <a name="see-also"></a>Voir aussi



[Référence EWS pour Exchange](ews-reference-for-exchange.md)

