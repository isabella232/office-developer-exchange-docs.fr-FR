---
title: Créer un agent de transport SmtpReceiveAgent pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Découvrez comment créer un agent de transport SmtpReceiveAgent personnalisé à utiliser avec Exchange 2013.
ms.openlocfilehash: a74d5baae6334c5e17acb6335206964b48f320e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755241"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>Créer un agent de transport SmtpReceiveAgent pour Exchange 2013

Découvrez comment créer un agent de transport SmtpReceiveAgent personnalisé à utiliser avec Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Extraits de code connexes et des exemples d’applications :

- [Exchange 2013 : Créer un agent de transport de conversion du corps](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
Les classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) permettent d’étendre le comportement du service de Transport frontal sur un serveur d’accès au Client ou le service de Transport sur un serveur de boîtes aux lettres. Vous pouvez utiliser ces classes pour implémenter des agents de transport qui sont conçus pour répondre aux messages lorsqu’ils sont dans votre organisation. 
  
Les classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) contiennent les événements répertoriés dans le tableau suivant. 
  
**Le tableau 1. Événements de la classe SmtpReceiveAgent**

|**Événement**|**Description**|
|:-----|:-----|
|[OnAuthCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |À utiliser lorsque votre agent nécessite des informations qui sont fournies uniquement dans la commande SMTP **AUTH** , comme un agent qui accepte ou rejette tente de remettre un message en fonction du type de méthode d’authentification utilisée.  <br/> |
|[OnConnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |À utiliser lorsque votre agent nécessite des informations qui sont fournies uniquement lors de l’ouverture d’une connexion via SMTP pour le service de Transport frontal, comme un agent qui effectue une action en fonction de l’adresse ou le domaine du serveur SMTP distant.  <br/> |
|[OnDataCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |Utilisez cet événement lorsque votre agent nécessite des informations fournies dans la commande SMTP **données** .  <br/> |
|[OnDisconnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |À utiliser lorsque votre agent nécessite des informations qui sont disponibles au moment de la déconnexion, telles que la date et l’heure, afin d’effectuer des calculs de temps.  <br/> |
|[OnEhloCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |À utiliser lorsque votre agent nécessite des informations fournies dans la commande SMTP **EHLO** ; par exemple, si votre agent accepte ou rejette les messages en fonction de l’identité fournie dans la commande **EHLO** .  <br/> |
|[OnEndOfAuthentication](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |À utiliser lorsque votre agent nécessite des informations qui sont disponibles une fois le serveur distant termine le processus d’authentification ; par exemple, pour un agent qui effectue une action sur un message en fonction des informations d’authentification fournies par le client ou le serveur SMTP distant.  <br/> |
|[OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |À utiliser lorsque votre agent doit effectuer une action en fonction des données qui sont disponibles dans le message. Cet événement se déclenche pas sur le service de Transport frontal. Si l’agent de transport a utiliser cet événement, vous devez l’installer sur un serveur de boîtes aux lettres.  <br/> |
|[OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |À utiliser lorsque votre agent doit effectuer une action en fonction des informations qui est disponibles dans les en-têtes du message envoyé.  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a>Création d’un agent de transport SmtpReceiveAgent personnalisé

La procédure suivante explique comment créer un agent de transport SmtpReceiveAgent personnalisé. 
  
### <a name="to-create-the-transport-agent"></a>Pour créer l’agent de transport

1. Ajoutez des références aux espaces de noms.
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   Vous trouverez ces espaces de noms sur votre serveur Exchange 2013. Lorsque vous ajoutez une référence à ces espaces de noms, vous avez accès aux membres [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) ainsi que d’autres classes utilisées dans le [Exchange 2013 : créer un agent de transport de conversion de corps](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) exemple. 
    
2. Implémenter la classe dérivée de la classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) . 
    
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

   Ce code instancie la classe dérivée et substituer la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé. 
    
3. Définir votre agent.
    
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

   Une fois que vous définissez votre classe agent, vous pouvez ajouter des fonctionnalités personnalisées. Dans cet exemple, l’événement [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) est redirigé vers votre gestionnaire d’événements personnalisé. 
    
## <a name="see-also"></a>Voir aussi

- [Concepts de l’agent d’Exchange 2013 de transport](transport-agent-concepts-in-exchange-2013.md)    
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

