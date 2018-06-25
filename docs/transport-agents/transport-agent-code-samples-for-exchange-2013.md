---
title: Exemples de code de l’agent pour Exchange 2013 de transport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: Trouvez des informations sur les agents de transport exemple disponibles pour Exchange 2013.
ms.openlocfilehash: 122a3351748fa6ffd823a51ce65ffb913332cb2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755142"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Exemples de code de l’agent pour Exchange 2013 de transport

Trouvez des informations sur les agents de transport exemple disponibles pour Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Vous pouvez utiliser les API qui sont inclus dans Exchange Server 2013 pour développer des agents qui étendent les fonctionnalités de transport. Cet article fournit des informations sur les agents d’exemples qui sont disponibles pour vous aider à apprendre à étendre le comportement du transport par programme. Les agents exemple incluent le code source pour chaque composant. 
  
Le tableau suivant répertorie les agents d’exemple pour Exchange 2013.
  
**Le tableau 1. Exemples de l’agent de transport**

|**Exemple de nom**|**Description**|
|:-----|:-----|
|[Exchange 2013 : Créer un agent de transport antivirus](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |Cet agent répond aux événements [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) et [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) et envoie un message entrant vers un serveur out-of-process qui examine le message de manière asynchrone et renvoie une version modifiée.  <br/> |
|[Exchange 2013 : Créer un agent de transport de journalisation de bande passante](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |Cet agent répond aux événements [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) et [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) , capture la bande passante pour les destinataires spécifiés et consigne les informations d’utilisation de la bande passante dans un fichier texte.  <br/> |
|[Exchange 2013 : Créer un agent de transport de conversion du corps](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |Cet agent de filtre les scripts de messages électroniques en définissant le format du message entrant et décider si le filtrage doit avoir lieu. Si le filtrage est nécessaire, le contenu est conversion au format HTML filtré et puis converti au format source.  <br/> |
|[Exchange 2013 : Créer un agent de transport de journalisation SMTP](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |Cet agent répond à l’événement [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) et asynchrone enregistre le message vers un fichier sur le disque dur local.  <br/> |
|[Exchange 2013 : Créer un agent de transport qui bloque temporairement des expéditeurs](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |Cet agent répond aux événements [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) et [OnRcptCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx) et détermine si l’expéditeur du message a déjà envoyé des messages au service de Transport frontal. Si l’expéditeur n'a pas déjà envoyé un message au service de Transport frontal, l’expéditeur est ajouté à une liste d’expéditeurs, et le message est rejeté à une réponse qui indique au client d’essayer ultérieurement (également appelé listes grises). Si l’expéditeur figure dans la liste des expéditeurs précédentes, l’agent de ne pas rejette le message.  <br/> |
|[Exchange 2013 : Créer un agent de transport enregistrement de serveur de boîtes aux lettres](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |Cet agent répond à l’événement de pipeline de transport [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) et enregistre de façon synchrone le message vers un fichier sur le disque dur local.  <br/> |
|[Exchange 2013 : Créer un agent de transport en-tête X](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |Cet agent répond à l’événement [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) et lire et modifier les en-têtes X dans les messages.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Concepts de l’agent d’Exchange 2013 de transport](transport-agent-concepts-in-exchange-2013.md)    
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [Créer un agent de transport RoutingAgent pour Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [Créer un agent de transport SmtpReceiveAgent pour Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [Créer un agent de transport DeliveryAgent pour Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

