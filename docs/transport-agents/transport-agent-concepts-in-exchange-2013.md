---
title: Concepts sur les agents de transport dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0c700af8-2792-4d3f-8571-8860e0550d8e
description: Découvrez comment l’architecture du pipeline d’agent de transport et du rôle serveur dans Exchange 2013 affecte le développement d’agents de transport et les classes que vous pouvez utiliser pour développer des agents de transport.
ms.openlocfilehash: 9116c9b7811958a2479421a642052df3cee24e34
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537160"
---
# <a name="transport-agent-concepts-in-exchange-2013"></a>Concepts sur les agents de transport dans Exchange 2013

Découvrez comment l’architecture du pipeline d’agent de transport et du rôle serveur dans Exchange 2013 affecte le développement d’agents de transport et les classes que vous pouvez utiliser pour développer des agents de transport. 
  
**S’applique à :** Exchange Server 2013 
  
Vous pouvez utiliser la bibliothèque de classes fournie dans Exchange Server 2013 pour implémenter des agents de transport qui s’inscrivent aux événements et prennent des mesures sur les messages lors de leur passage via le pipeline de transport. Vous pouvez également utiliser des agents de transport pour modifier des messages et convertir du contenu. 
  
Cet article fournit des informations sur les agents de transport et l’architecture de pipeline de transport. Il est important de comprendre l’architecture du pipeline de transport pour pouvoir modifier le comportement de transport de manière adaptée aux besoins de votre organisation. Cet article fournit également des informations sur les modifications apportées à l’architecture d’Exchange 2013 qui ont des répercussions sur les agents de transport et les classe que vous pouvez utiliser pour développer des agents de transport.  
  
## <a name="transport-agents-in-the-transport-pipeline"></a>Agents de transport dans le pipeline de transport
<a name="Pipeline"> </a>

Les agents de transport sont issus d’une des trois catégories suivantes :
  
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
- [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx)
    
Le pipeline de transport fait référence au flux de données de messagerie, dans les limites d’une organisation Exchange 2013. Le pipeline se compose des services répertoriés dans le tableau suivant.
  
**Tableau 1. Services de pipeline de transport**

|**Service**|**Description**|**Classes prises en charge**|
|:-----|:-----|:-----|
|Transport frontal  <br/> |S’exécute [](https://technet.microsoft.com/library/dd298114%28v=exchg.150%29.aspx) sur tous les serveurs d’accès au client et agit comme un proxy sans état pour tout le trafic SMTP externe entrant et sortant pour l’organisation Exchange 2013. Le service de transport frontal n’inspecte pas le contenu des messages ni ne place ces derniers en file d’attente localement. Il communique avec le service de transport sur un serveur [de boîtes aux lettres.](https://technet.microsoft.com/library/jj150491%28v=exchg.150%29.aspx)  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Transport  <br/> |S’exécute sur tous les serveurs de boîtes aux lettres et est similaire au rôle serveur de [transport Hub](https://technet.microsoft.com/library/bb123494%28v=exchg.141%29.aspx) Exchange Server 2010. Le service de transport route les messages entre lui-même et les services de transport frontal et de transport de boîtes aux lettres. Ce service ne communique pas directement avec les bases de données de boîtes aux lettres.  <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) <br/> |
|Transport de boîtes aux lettres  <br/> |S’exécute sur tous les serveurs de boîtes aux lettres et se compose de deux services distincts : dépôt de transport de boîtes aux lettres et remise de transport de boîtes aux lettres. La remise de transport de boîtes aux lettres reçoit les messages SMTP du service de transport et se connecte à la base de données de boîtes aux lettres via un appel de procédure distante (RPC) Exchange pour livrer les messages. Le dépôt de transport de boîtes aux lettres se connecte à la base de données de boîtes aux lettres via un RPC pour récupérer les messages et les soumettre via SMTP au service de transport.  <br/> |Aucun.  <br/> |
   
### <a name="transport-events"></a>Événements de transport
<a name="Events"> </a>

Pour implémenter des agents de transport, vous devez tout d’abord l’enregistrer pour un événement, puis exécuter une action lorsque cet événement est déclenché. Chacun des trois types d’agent peut être enregistré pour un ensemble d’événements différent.
  
La figure suivante indique les emplacements du pipeline de transport où les agents de transport peuvent être enregistrés pour des événements.
  
**Figure 1. Événements de transport**

![Image présentant le flux de messages via le pipeline de transport et les événements auxquels chaque agent peut s’inscrire, en commençant par les événements SMPT pour SmtpReceivedAgent, puis les événements Categorizor pour RoutingAgent, et enfin les événements DELIVER pour DeliveryAgent.](media/TAConceptsFig1.png)
  
Lorsqu’un message entre dans le pipeline de transport, un agent de transport dérivé de la classe [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) peut agir sur le message pendant l’un des événements SMTP inscrits par l’agent. Un agent dérivé de la [classe RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) peut agir sur l’un des quatre événements de catégoriseur qu’il a inscrits. Un agent dérivé de la classe [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.aspx) peut agir sur un message pendant tous les événements de remise qu’il a enregistrés. 
  
## <a name="transport-agents-and-server-roles"></a>Rôles serveur et agents de transport
<a name="ServerRoles"> </a>

Les modifications apportées à l’architecture du rôle serveur Exchange 2013 affectent les agents de transport et ce que vos agents de transport peuvent faire. Exchange 2013 inclut les rôles serveur suivants :
  
- Serveur de boîtes aux lettres : inclut des protocoles d’accès au client, le service de transport, des bases de données de boîtes aux lettres et des composants de messagerie unifiée. Le serveur de boîtes aux lettres communique directement avec les services de domaine Active Directory (AD DS), les serveurs d’accès au client et des clients de messagerie comme Outlook.
    
- Serveur d’accès au client : fournit des services d’authentification, de redirection limitée et de proxy, ainsi que des protocoles d’accès au client comme HTTP, POP, IMAP et SMTP.
    
- Serveur de transport Edge : route les e-mails en direction et à partir d’une organisation. En règle générale, les serveurs de transport Edge se trouvent au niveau du périmètre d’une topologie Exchange.
    
Cette structure consolidée permet de réduire le nombre de serveurs qui doivent être déployés dans un environnement Exchange 2013. Les administrateurs n’ont plus à déployer des serveurs de transport Hub et d’accès au client dans chaque site Active Directory qui comprend un serveur de boîtes aux lettres, et ils n’ont plus besoin de mettre à jour tous les rôles serveur afin de bénéficier des nouvelles fonctionnalités.
  
Ces modifications apportées à l’architecture des rôles serveur peuvent potentiellement modifier l’emplacement du pipeline où votre agent peut répondre aux événements. Si vous avez créé des agents de transport pour des versions d’Exchange antérieures à Exchange 2013, passez en revue les modifications apportées à l’architecture pour déterminer si vous devez apporter des modifications à vos agents.
  
La figure suivante indique en quoi les changements d’architecture d’Exchange 2013 offrent un pipeline de transport simplifié et consolidé. Dans cette illustration, les serveurs d’accès au client sont représentés par les vignettes CAS. Les serveurs de boîtes aux lettres sont eux représentés par les vignettes MBX.
  
**Figure 2. Exchange 2013 server role architecture**

![Image illustrant le trafic client via un pare-feu externe et le transport Edge sur la gauche qui transmet le trafic par le biais d’un équilibrage de charge de couche 4 vers un tableau CAS consolidé et un ensemble de serveurs de boîtes aux lettres dans un groupe d’accessibilité de base de données sur la droite.](media/Transport_Agent_Concepts_Fig_3.png)
  
La figure suivante illustre les interactions entre les rôles serveur Exchange 2013.
  
**Figure 3. Interactions entre les serveurs de boîtes aux lettres et d’accès au client**

![Image présentant les interactions en débutant avec des flèches à partir du trafic client passant à travers un équilibrage de charge de couche 4 qui possède 4 cibles dans le tableau CAS : IIS/proxy HTTP, POP/IMAP, SMTP et messagerie unifiée. Les flèches passent vers leurs cibles complémentaires dans la banque de boîtes aux lettres.](media/Transport_Agent_Concepts_Fig_4.png)
  
Pour plus d’informations sur les modifications apportées à l’architecture de rôle serveur Exchange 2013, voir [Exchange 2013 architecture](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx#BKMK_Arch) in [What’s New in Exchange 2013](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx). 
  
## <a name="transport-agent-classes"></a>Classes d’agent de transport
<a name="Create"> </a>

La classe dont votre agent de transport est dérivé détermine les événements pour lesquels votre agent peut être enregistré. Votre agent contient généralement une classe d’agent, une fabrique d’agent, un ou plusieurs gestionnaires d’événements, ainsi que le code qui effectue les actions que vous voulez que votre agent applique.
  
Le tableau suivant indique les classes à partir desquelles chaque type d’agent est dérivé.
  
**Tableau 2. Classes d’agent**

||||
|:-----|:-----|:-----|
|Type d’agent  <br/> |Classe de base de fabrique  <br/> |Classe de base d’agent  <br/> |
|Réception SMTP  <br/> |[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) <br/> |[SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) <br/> |
|Routage  <br/> |[RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) <br/> |[RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) <br/> |
|Remise  <br/> |[DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) <br/> |[DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) <br/> |
   
Ces classes de base de fabrique et d’agent fournissent des propriétés et les méthodes que vous pouvez utiliser pour accéder à des messages et à des événements de transport. Mettez en œuvre des classes qui héritent de celles-ci dans votre agent. Dans la classe dérivée de la fabrique d’agent, remplacez la méthode **CreateAgent** afin qu’elle renvoie une nouvelle instance de votre classe d’agent. 
  
Les arguments transmis aux événements peuvent contenir une instance de la classe [EmailMessage,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailMessage.aspx) que vous pouvez utiliser pour modifier les propriétés et le contenu du message sous-jacent. Toutes les informations du message sont disponibles dans chaque événement. Vous devez déterminer l’agent et l’événement qui conviennent le mieux à la tâche que vous voulez accomplir. 
  
Les espaces de noms suivants contiennent des types qui vous permettent de lire, d’écrire et de modifier des messages dans le pipeline de transport :
  
- [Microsoft. Exchange. Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx)
    
- [Microsoft. Exchange. Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx)
    
- [Microsoft. Exchange. Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx)
    
- [Microsoft. Exchange. Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx)
    
- [Microsoft. Exchange. Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx)
    
Après avoir écrit votre agent de transport, vous installez et gérez votre [agent](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx) à l’aide de Exchange Management Shell. Pour plus d’informations, voir [Creating transport agents for Exchange 2013](creating-transport-agents-for-exchange-2013.md). 
  
## <a name="see-also"></a>Voir aussi

- [Agents de transport dans Exchange](transport-agents-in-exchange-2013.md)    
- [Référence de l’agent de transport Exchange 2013](transport-agent-reference-for-exchange-2013.md)   
- [Lecture et modification de messages dans le pipeline de transport Exchange 2013](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)    
- [Nouveautés de Exchange 2013](https://technet.microsoft.com/library/jj150540%28v=exchg.150%29.aspx)   
- [Exchange 2013 Server Role Architecture](https://blogs.technet.com/b/exchange/archive/2013/01/23/exchange-2013-server-role-architecture.aspx)    
- [Serveurs de boîtes aux lettres et d’accès au client](https://technet.microsoft.com/library/jj150519%28v=exchg.150%29.aspx)   
- [Exchange Server 2013 Mail Flow](https://technet.microsoft.com/library/aa996349.aspx)
- [Exchange Server 2013 Mail Routing](https://technet.microsoft.com/library/aa998825%28v=exchg.150%29.aspx)   
- [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
    

