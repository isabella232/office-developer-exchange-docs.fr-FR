---
title: Concepts sur les agents de transport dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0c700af8-2792-4d3f-8571-8860e0550d8e
description: Trouvez des informations sur l’architecture de rôle transport agent pipeline et le serveur Exchange 2013 influence développement d’agent de transport et les classes que vous pouvez utiliser pour développer des agents de transport.
ms.openlocfilehash: 9ddee0d68c9104357f84322b2cce7c5f2576d871
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755147"
---
# <a name="transport-agent-concepts-in-exchange-2013"></a>Concepts sur les agents de transport dans Exchange 2013

Trouvez des informations sur l’architecture de rôle transport agent pipeline et le serveur Exchange 2013 influence développement d’agent de transport et les classes que vous pouvez utiliser pour développer des agents de transport. 
  
**S’applique à :** Exchange Server 2013 
  
Vous pouvez utiliser la bibliothèque de classes fournie dans Exchange Server 2013 pour implémenter des agents de transport s’inscrire pour les événements et effectuer des actions sur les messages transitant via le pipeline de transport. Vous pouvez également utiliser des agents de transport pour modifier les messages et convertir le contenu. 
  
Cet article fournit des informations sur les agents de transport et l’architecture de pipeline de transport. Il est important de comprendre l’architecture du pipeline de transport de sorte que vous pouvez modifier le comportement de transport pour répondre aux besoins de votre organisation. Cet article fournit également des informations sur les modifications dans l’architecture Exchange 2013 qui affectent les agents de transport et les classes que vous pouvez utiliser pour développer des agents de transport. 
  
## <a name="transport-agents-in-the-transport-pipeline"></a>Agents de transport dans le pipeline de transport
<a name="Pipeline"> </a>

Les agents de transport sont issus d’une des trois catégories suivantes :
  
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
- [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)
    
Le pipeline de transport fait référence au flux de données de messagerie, dans les limites d’une organisation Exchange 2013. Le pipeline se compose des services répertoriés dans le tableau suivant.
  
**Le tableau 1. Services de pipeline de transport**

|**Service**|**Description**|**Classes prises en charge**|
|:-----|:-----|:-----|
|Transport frontal   <br/> |S’exécute sur tous les [serveurs d’accès au Client](http://technet.microsoft.com/en-us/library/dd298114%28v=exchg.150%29.aspx) et agit comme un proxy pour le trafic entrant et sortant externe SMTP pour l’organisation Exchange 2013 sans état. Le service de Transport frontal n’inspecter le contenu des messages ou localement tous les messages des files d’attente. Il communique avec le service de Transport sur un [serveur de boîtes aux lettres](http://technet.microsoft.com/en-us/library/jj150491%28v=exchg.150%29.aspx).  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Transport  <br/> |S’exécute sur tous les serveurs de boîtes aux lettres et est similaire au rôle [serveur de Transport Hub](http://technet.microsoft.com/en-us/library/bb123494%28v=exchg.141%29.aspx) dans Exchange Server 2010. Le service de Transport achemine les messages entre lui-même et les services de Transport de boîtes aux lettres et de Transport frontal. Ce service ne communique pas directement avec les bases de données de boîtes aux lettres.  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
|Transport de boîtes aux lettres  <br/> |S’exécute sur tous les serveurs de boîtes aux lettres et se compose de deux services distincts : dépôt de Transport de boîtes aux lettres et de la remise de Transport de boîtes aux lettres. Remise de Transport de boîte aux lettres reçoit les messages SMTP à partir du service de Transport et se connecte à la base de données de boîtes aux lettres à l’aide d’un appel de procédure distante (RPC) Exchange pour remettre le message. Dépôt de Transport de boîtes aux lettres se connecte à la base de données de boîtes aux lettres à l’aide de RPC pour récupérer des messages et envoie les messages via SMTP pour le service de Transport.  <br/> |Aucune.  <br/> |
   
### <a name="transport-events"></a>Événements de transport
<a name="Events"> </a>

Pour implémenter des agents de transport, vous devez tout d’abord l’enregistrer pour un événement, puis exécuter une action lorsque cet événement est déclenché. Chacun des trois types d’agent peut être enregistré pour un ensemble d’événements différent.
  
La figure suivante indique les emplacements du pipeline de transport où les agents de transport peuvent être enregistrés pour des événements.
  
**La figure 1. Événements de transport**

![Image présentant le flux de messages via le pipeline de transport et les événements auxquels chaque agent peut s’inscrire, en commençant par les événements SMPT pour SmtpReceivedAgent, puis les événements Categorizor pour RoutingAgent, et enfin les événements DELIVER pour DeliveryAgent.](media/TAConceptsFig1.png)
  
Lorsqu’un message entre dans le pipeline de transport, un agent de transport dérivé de la classe [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) peut agir sur le message pendant les événements enregistrés par l’agent pour SMTP. Un agent dérivé de la classe [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) peut agir sur un des quatre événements enregistré par catégoriseur. Un agent dérivé de la classe [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) peut agir sur un message pendant les événements de la remise enregistré par. 
  
## <a name="transport-agents-and-server-roles"></a>Rôles serveur et agents de transport
<a name="ServerRoles"> </a>

Modifications apportées à l’architecture du rôle serveur dans Exchange 2013 affectent ce que peuvent faire les agents de transport et les agents de transport. Exchange 2013 comprend les rôles de serveur suivants :
  
- Serveur de boîtes aux lettres — protocoles inclut l’accès au Client, le service de Transport, bases de données de boîtes aux lettres et composants de messagerie unifiée. Le serveur de boîtes aux lettres communique directement avec les Services de domaine Active Directory (AD DS), les serveurs d’accès Client et les clients de messagerie comme Outlook.
    
- Serveur d’accès au client : fournit des services d’authentification, de redirection limitée et de proxy, ainsi que des protocoles d’accès au client comme HTTP, POP, IMAP et SMTP.
    
- Serveur de transport Edge : route les e-mails en direction et à partir d’une organisation. En règle générale, les serveurs de transport Edge se trouvent au niveau du périmètre d’une topologie Exchange.
    
Cette structure consolidée réduit le nombre de serveurs qui doivent être déployés dans un environnement Exchange 2013. Les administrateurs n’ont plus à déployer des serveurs de Transport Hub et d’accès au Client dans chaque site Active Directory qui comprend un serveur de boîtes aux lettres, et ils n’avez plus besoin mettre à jour tous les rôles de serveur afin de tirer parti des nouvelles fonctionnalités.
  
Ces modifications à l’architecture du rôle serveur peuvent affecter potentiellement où dans le pipeline de l’agent peut répondre aux événements. Si vous avez créé des agents de transport pour les versions d’Exchange antérieures à Exchange 2013, veillez à consulter les modifications architecturales pour déterminer si vous devez apporter des modifications à vos agents.
  
La figure suivante indique en quoi les changements d’architecture d’Exchange 2013 offrent un pipeline de transport simplifié et consolidé. Dans cette illustration, les serveurs d’accès au client sont représentés par les vignettes CAS. Les serveurs de boîtes aux lettres sont eux représentés par les vignettes MBX.
  
**La figure 2. Architecture du rôle serveur Exchange 2013**

![Image illustrant le trafic client via un pare-feu externe et le transport Edge sur la gauche qui transmet le trafic par le biais d’un équilibrage de charge de couche 4 vers un tableau CAS consolidé et un ensemble de serveurs de boîtes aux lettres dans un groupe d’accessibilité de base de données sur la droite.](media/Transport_Agent_Concepts_Fig_3.png)
  
La figure suivante illustre les interactions entre les rôles de serveur Exchange 2013.
  
**La figure 3. Interactions de serveur de boîtes aux lettres et accès au Client**

![Image présentant les interactions en débutant avec des flèches à partir du trafic client passant à travers un équilibrage de charge de couche 4 qui possède 4 cibles dans le tableau CAS : IIS/proxy HTTP, POP/IMAP, SMTP et messagerie unifiée. Les flèches passent vers leurs cibles complémentaires dans la banque de boîtes aux lettres.](media/Transport_Agent_Concepts_Fig_4.png)
  
Pour plus d’informations sur les modifications apportées à l’architecture du rôle serveur Exchange 2013, voir [architecture Exchange 2013](http://technet.microsoft.com/en-us/library/jj150540%28v=exchg.150%29.aspx#BKMK_Arch) dans [Nouveautés dans Exchange 2013](http://technet.microsoft.com/en-us/library/jj150540%28v=exchg.150%29.aspx). 
  
## <a name="transport-agent-classes"></a>Classes d’agent de transport
<a name="Create"> </a>

La classe dont votre agent de transport est dérivé détermine les événements pour lesquels votre agent peut être enregistré. Votre agent contient généralement une classe d’agent, une fabrique d’agent, un ou plusieurs gestionnaires d’événements, ainsi que le code qui effectue les actions que vous voulez que votre agent applique.
  
Le tableau suivant indique les classes à partir desquelles chaque type d’agent est dérivé.
  
**Le tableau 2. Classes de l’agent**

||||
|:-----|:-----|:-----|
|Type d’agent  <br/> |Classe de base de fabrique  <br/> |Classe de base d’agent  <br/> |
|Réception SMTP  <br/> |[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Routage  <br/> |[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) <br/> |[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> |
|Remise  <br/> |[DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) <br/> |[DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
   
Ces classes de base en usine et agent fournissent des propriétés et méthodes que vous pouvez utiliser pour accéder aux événements de transport et des messages. Implémenter les classes dans l’agent qui héritent de ces classes. Dans la classe dérivée de fabrique agent, substituez la méthode de **CreateAgent** afin qu’elle retourne une nouvelle instance de votre classe de l’agent. 
  
Les arguments transmis aux événements peuvent contenir une instance de la classe [EmailMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailMessage.aspx) , que vous pouvez utiliser pour modifier les propriétés et le contenu du message sous-jacent. Toutes les informations de message sont disponibles dans chaque événement. Vous devez déterminer de l’agent et l’événement qui convient le mieux à la tâche que vous souhaitez effectuer. 
  
Les espaces de noms suivants contiennent des types qui vous permettent de lire, d’écrire et de modifier des messages dans le pipeline de transport :
  
- [Microsoft.Exchange.Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx)
    
- [Microsoft.Exchange.Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx)
    
- [Microsoft.Exchange.Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx)
    
- [Microsoft.Exchange.Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx)
    
- [Microsoft.Exchange.Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx)
    
Une fois que vous écrivez votre agent de transport, vous [installer et gérer votre agent](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx) à l’aide de l’environnement Exchange Management Shell. Pour plus d’informations, voir [création des agents de transport pour Exchange 2013](creating-transport-agents-for-exchange-2013.md). 
  
## <a name="see-also"></a>Voir aussi

- [Agents de transport dans Exchange](transport-agents-in-exchange-2013.md)    
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)   
- [Lecture et de modification des messages dans le pipeline de transport Exchange 2013](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)    
- [Quelles sont les nouveautés dans Exchange 2013](http://technet.microsoft.com/en-us/library/jj150540%28v=exchg.150%29.aspx)   
- [Architecture de rôle de serveur Exchange 2013](http://blogs.technet.com/b/exchange/archive/2013/01/23/exchange-2013-server-role-architecture.aspx)    
- [Boîte aux lettres et les serveurs d’accès au Client](http://technet.microsoft.com/en-us/library/jj150519%28v=exchg.150%29.aspx)   
- [Flux de messagerie Exchange Server 2013](http://technet.microsoft.com/en-us/library/aa996349.aspx)
- [Le routage Exchange Server 2013 messagerie](http://technet.microsoft.com/en-us/library/aa998825%28v=exchg.150%29.aspx)   
- [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
    

