---
title: Éléments du fichier de configuration des agents pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Agents
api_type:
- schema
ms.assetid: 3047653b-d712-46c1-ae0a-73f3975f5e9d
description: Recherchez des informations sur les éléments XML dans le fichier de configuration agents. config et fetagents. config dans Exchange 2013.
ms.openlocfilehash: f19fe8316a78cef668db881e630562d3be8be64a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461568"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Éléments du fichier de configuration des agents pour Exchange 2013

Recherchez des informations sur les éléments XML dans le fichier de configuration agents. config et fetagents. config dans Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Lorsque vous installez le rôle serveur d’accès au client ou de boîte aux lettres sur un serveur Exchange, le programme d’installation crée un fichier XML qui contient des informations de configuration sur les agents installés sur le serveur. Vous ne pouvez pas écrire directement dans ce fichier. 
  
Le service de transport frontal s’exécute sur les serveurs d’accès au client et écrit dans un fichier nommé fetagents. config. Le service de transport et le service de transport de boîtes aux lettres s’exécutent sur des serveurs de boîtes aux lettres, et sont écrits dans un fichier nommé agents. config. Un ordinateur qui a à la fois le rôle serveur d’accès au client et le rôle serveur de boîte aux lettres aura à la fois un fichier fetagents. config et un fichier agents. config. 
  
La seule façon d’écrire dans ces fichiers est d’utiliser les applets de commande de l’agent de transport dans l’environnement de commande Exchange Management Shell. Pour plus d’informations sur les applets de commande de l’agent de transport, consultez la rubrique [mail Flow cmdlets](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) on technet. 
  
> [!NOTE]
> Pour faire la distinction entre les agents qui étendent le service de transport frontal sur le serveur d’accès au client et le service de transport sur le serveur de boîtes aux lettres, les cmdlets de l’agent de transport ont un paramètre _TransportService_ avec la valeur « Hub » pour le service de transport et « frontend » pour le service de transport frontal. 
  
Vous pouvez lire le fichier agents. config ou fetagents. config pour déterminer la présence et les informations de configuration d’un ou de plusieurs agents sur le serveur. Cette documentation fournit une référence que vous pouvez utiliser pour lire les informations dans le fichier agents. config ou fetagents. config. Le format de ces deux fichiers est le même. Cette documentation ne fournit pas d’informations sur la façon d’écrire dans les fichiers.
  
> [!CAUTION]
> L’utilisation de méthodes non prises en charge pour écrire dans le fichier agents. config ou fetagents. config peut produire des résultats inattendus, notamment l’échec du service de transport ou des agents de transport, ou les deux. N’écrivez pas directement dans l’un de ces fichiers. La seule méthode prise en charge pour l’écriture dans ces fichiers est d’utiliser les cmdlets de l’agent de transport de l’environnement de commande Exchange Management Shell. 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>Emplacement des fichiers de configuration de l’agent de transport
<a name="bk_ConfigLoc"> </a>

Lorsque vous installez Exchange 2013, le programme d’installation crée un fichier XML nommé agents. config. template ou fetagents. config. Template, selon le rôle serveur installé, dans le \<ExchangeInstallFolder\> dossier \TransportRoles\Agents (où \<ExchangeInstallFolder\> est le dossier dans lequel vous avez installé Exchange 2013). Si vous installez le rôle serveur d’accès au client, Exchange 2013 copie le fichier fetagents. config. template dans fetagents. config. Si vous installez le rôle serveur de boîtes aux lettres, Exchange 2013 copie le fichier agents. config. template dans agents. config. Exchange 2013 lit et écrit ce fichier lorsque vous modifiez la configuration des agents de transport sur le serveur.
  
## <a name="verifying-a-transport-agent-installation"></a>Vérification de l’installation d’un agent de transport
<a name="bk_verifyinstall"> </a>

Vous pouvez utiliser les fonctionnalités XML fournies par .NET Framework pour lire et valider le fichier agents. config ou le fichier XML fetagents. config. Pour vérifier l’installation et la configuration d’un agent de transport, lisez le code XML dans le fichier de configuration et recherchez l’élément [agent](agent.md) correspondant à l’agent de transport. Si un élément **agent** pour l’agent de transport spécifique n’existe pas, l’agent de transport n’est pas installé. Si l’agent de transport est installé, vous pouvez lire les attributs de l’élément **agent** pour en déterminer la configuration. 
  
## <a name="configuration-file-element-hierarchy"></a>Hiérarchie des éléments du fichier de configuration
<a name="bk_elementref"> </a>

Le code suivant montre la hiérarchie des éléments dans le fichier XML de configuration.
  
```XML
<configuration>
    <mexRuntime>
        <monitoring>
            <agentExecution/>
            <messageSnapshot/>
        </monitoring>
        <agentList>
            <agent/>
            <agent/>
            <agent />
        </agentList>
    </mexRuntim>
</configuration>
```

## <a name="in-this-section"></a>Dans cette section
<a name="bk_elementreflist"> </a>

- [agent](agent.md)
    
- [agentExecution](agentexecution.md)
    
- [agentList](agentlist.md)
    
- [configuration](configuration.md)
    
- [messageSnapshot](messagesnapshot.md)
    
- [mexRuntime](mexruntime.md)
    
- [surveillance](monitoring.md)
    
## <a name="see-also"></a>Voir aussi

- [Agents de transport dans Exchange](transport-agents-in-exchange-2013.md)
- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)
- [Espaces de noms de l’agent de transport dans Exchange 2013](transport-agent-namespaces-in-exchange-2013.md)
- [Cmdlets de flux de messagerie](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

