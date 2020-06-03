---
title: Création d’un agent de transport SmtpReceiveAgent pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Découvrez comment créer un agent de transport SmtpReceiveAgent personnalisé à utiliser avec Exchange 2013.
ms.openlocfilehash: 5ba021d02849ffc7e125029f0fd18ebf14c3f8da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459138"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>Création d’un agent de transport SmtpReceiveAgent pour Exchange 2013

Découvrez comment créer un agent de transport SmtpReceiveAgent personnalisé à utiliser avec Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Extraits de code et exemples d’applications connexes :

- [Exchange 2013 : création d’un agent de transport de conversion corporelle](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
Les classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) vous permettent d’étendre le comportement du service de transport frontal sur un serveur d’accès au client ou le service de transport sur un serveur de boîtes aux lettres. Vous pouvez utiliser ces classes pour implémenter des agents de transport qui sont conçus pour répondre aux messages au fur et à mesure qu’ils arrivent dans votre organisation. 
  
Les classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) incluent les événements présentés dans le tableau suivant. 
  
**Tableau 1. Événements de classe SmtpReceiveAgent**

|**Event**|**Description**|
|:-----|:-----|
|[OnAuthCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |À utiliser lorsque votre agent requiert des informations fournies uniquement dans la commande SMTP **auth** , comme un agent qui accepte ou rejette les tentatives de remise d’un message en fonction du type de méthode d’authentification utilisée.  <br/> |
|[OnConnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |À utiliser lorsque votre agent nécessite des informations fournies uniquement lorsqu’une connexion est ouverte via SMTP vers le service de transport frontal, tel qu’un agent qui effectue une action basée sur l’adresse ou le domaine du serveur SMTP distant.  <br/> |
|[OnDataCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |Utilisez cet événement lorsque votre agent requiert des informations fournies dans la commande de **données** SMTP.  <br/> |
|[OnDisconnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |À utiliser lorsque votre agent requiert des informations qui sont disponibles au moment de la déconnexion, telles que la date et l’heure actuelles, afin d’effectuer des calculs de temps.  <br/> |
|[OnEhloCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |À utiliser lorsque votre agent requiert des informations fournies dans la commande SMTP **EHLO** ; par exemple, si votre agent accepte ou rejette les messages en fonction de l’identité fournie dans la commande **EHLO** .  <br/> |
|[OnEndOfAuthentication](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |À utiliser lorsque votre agent requiert des informations qui sont disponibles après que le serveur distant a terminé le processus d’authentification ; par exemple, pour un agent qui effectue une action sur un message en fonction des informations d’authentification fournies par le serveur ou le client SMTP distant.  <br/> |
|[OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |À utiliser lorsque votre agent doit effectuer une action basée sur les données disponibles dans le message. Cet événement ne se déclenche pas sur le service de transport frontal. Si votre agent de transport doit utiliser cet événement, vous devez l’installer sur un serveur de boîtes aux lettres.  <br/> |
|[OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |À utiliser lorsque votre agent doit effectuer une action basée sur les informations disponibles dans les en-têtes du message envoyé.  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a>Création d’un agent de transport SmtpReceiveAgent personnalisé

La procédure suivante décrit comment créer un agent de transport SmtpReceiveAgent personnalisé. 
  
### <a name="to-create-the-transport-agent"></a>Pour créer l’agent de transport

1. Ajoutez des références aux espaces de noms.
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   Ces espaces de noms se trouvent sur votre serveur Exchange 2013. Lorsque vous ajoutez une référence à ces espaces de noms, vous avez accès aux membres du [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) , ainsi qu’aux autres classes utilisées dans l’exemple [Exchange 2013 : Build a Body conversion agent](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) . 
    
2. Implémentez la classe dérivée pour la classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) . 
    
   ```cs
      public class BodyConversionFactory : SmtpReceiveAgentFactory
      {
          /// <summary>
          /// Create a new BodyConversion
          /// </summary>
          /// <param name="server">Exchange server</param>
          /// <returns>A new BodyConversion</returns>
          public override SmtpReceiveAgent CreateAgent(SmtpServer server)
          {
              return new BodyConversion();
          }
      }
  
   ```

   Ce code instancie la classe dérivée et remplace la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé. 
    
3. Définissez votre agent.
    
   ```cs
     public class BodyConversion : SmtpReceiveAgent
      {
          // Your custom code goes here
          /// <summary>
          /// The constructor registers an end of data event handler.
          /// </summary>
          public BodyConversion()
          {
              Debug.WriteLine("[BodyConversion] Agent constructor");
              this.OnEndOfData += new EndOfDataEventHandler(this.OnEndOfDataHandler);
          }
      }
  
   ```

   Une fois que vous avez défini votre classe d’agent, vous pouvez ajouter vos fonctionnalités personnalisées. Dans cet exemple, l’événement [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) est redirigé vers votre gestionnaire d’événements personnalisé. 
    
## <a name="see-also"></a>Voir aussi

- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

