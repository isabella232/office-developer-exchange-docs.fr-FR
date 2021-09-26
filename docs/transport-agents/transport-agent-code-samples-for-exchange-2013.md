---
title: Exemples de code d’agent de transport Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: Trouvez des informations sur les exemples d’agents de transport disponibles Exchange 2013.
ms.openlocfilehash: 56334f661947cffceaf18eb257feeb6504a71ecb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545710"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Exemples de code d’agent de transport Exchange 2013

Trouvez des informations sur les exemples d’agents de transport disponibles Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Vous pouvez utiliser les API incluses dans Exchange Server 2013 pour développer des agents qui étendent les fonctionnalités de transport. Cet article fournit des informations sur les exemples d’agents disponibles pour vous aider à apprendre à étendre le comportement de transport par programme. Les exemples d’agents incluent le code source de chaque composant. 
  
Le tableau suivant répertorie les exemples d’agents Exchange 2013.
  
**Tableau 1. Exemples d’agent de transport**

|**Exemple de nom**|**Description**|
|:-----|:-----|
|[Exchange 2013 : Créer un agent de transport antivirus](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |Cet agent répond aux événements [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) et [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) et envoie le message entrant à un serveur hors processus qui examine le message de manière asynchrone et retourne une version modifiée.  <br/> |
|[Exchange 2013 : Créer un agent de transport de journalisation de la bande passante](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |Cet agent répond aux événements [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) et [OnRoutedMessage,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) capture l’utilisation de la bande passante pour les destinataires spécifiés et enregistre les informations d’utilisation de la bande passante dans un fichier texte.  <br/> |
|[Exchange 2013 : Créer un agent de transport de conversion de corps](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |Cet agent filtre les scripts des messages électroniques en déterminant le format du message entrant et en déterminant si le filtrage doit avoir lieu. Si le filtrage est nécessaire, le contenu est converti au format HTML, filtré, puis reconverti au format source.  <br/> |
|[Exchange 2013 : Créer un agent de transport de journalisation SMTP](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |Cet agent répond à l’événement [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) et enregistre le message de manière asynchrone dans un fichier sur le disque dur local.  <br/> |
|[Exchange 2013 : créer un agent de transport qui bloque temporairement les expéditeurs](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |Cet agent répond aux événements [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) et [OnRcptCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx) et détermine si l’expéditeur du message a déjà envoyé des messages au service de transport frontal. Si l’expéditeur n’a pas encore envoyé de message au service de transport frontal, l’expéditeur est ajouté à une liste d’expéditeurs et le message est rejeté avec une réponse qui indique au client de réessayer ultérieurement (également appelée « liste grise »). Si l’expéditeur figure dans la liste des expéditeurs précédents, l’agent ne rejette pas le message.  <br/> |
|[Exchange 2013 : Créer un agent de transport de journalisation de serveur de boîtes aux lettres](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |Cet agent répond à l’événement de pipeline de transport [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) et enregistre de manière synchrone le message dans un fichier sur le disque dur local.  <br/> |
|[Exchange 2013 : Créer un agent de transport d’en-tête X](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |Cet agent répond à [l’événement OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) et lit et modifie les en-têtes X dans les messages.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Référence de l’agent de transport Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [Créer un agent de transport RoutingAgent pour Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [Créer un agent de transport SmtpReceiveAgent pour Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [Créer un agent de transport DeliveryAgent pour Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

