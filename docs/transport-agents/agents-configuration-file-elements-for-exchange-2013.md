---
title: Éléments du fichier de configuration agents pour Exchange 2013
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
description: Trouvez des informations sur les éléments XML dans le fichier de configuration fetagents.config et les versions d’Exchange 2013.
ms.openlocfilehash: dd58c4bc21a968db2ca5b13e0c53f7058b29f233
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755120"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Éléments du fichier de configuration agents pour Exchange 2013

Trouvez des informations sur les éléments XML dans le fichier de configuration fetagents.config et les versions d’Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Lorsque vous installez l’accès au Client ou le rôle serveur de boîtes aux lettres sur un serveur Exchange, le programme d’installation crée un fichier XML qui contient les informations de configuration des agents qui sont installés sur le serveur. Vous ne pouvez pas écrire directement à ce fichier. 
  
Le service de Transport frontal s’exécute sur des serveurs d’accès au Client et écrit dans un fichier nommé fetagents.config. Le service de Transport et le service de Transport de boîtes aux lettres s’exécutent sur des serveurs de boîtes aux lettres et écrire dans un fichier nommé versions. Un ordinateur ayant le rôle de serveur d’accès au Client et du rôle serveur de boîtes aux lettres aura à la fois un fetagents.config et un fichier de versions. 
  
Il est le seul moyen pris en charge pour écrire dans ces fichiers en utilisant les applets de commande de l’agent de transport dans Exchange Management Shell. Pour plus d’informations sur les applets de commande de l’agent de transport, voir [Applets de commande de flux de messagerie](http://technet.microsoft.com/en-us/library/aa998553%28v=exchg.150%29.aspx) sur TechNet. 
  
> [!NOTE]
> Pour faire la distinction entre les agents qui étendent le service de Transport frontal sur le serveur d’accès au Client et le service de Transport sur le serveur de boîtes aux lettres, cmdlets d’agent de transport ont un paramètre _TransportService_ avec la valeur « Hub » pour le Transport service et « FrontEnd » pour le service de Transport frontal. 
  
Vous pouvez lire des versions ou fichier fetagents.config pour déterminer la présence des informations de configuration pour un ou plusieurs agents sur le serveur. Cette documentation fournit une référence que vous pouvez utiliser pour lire les informations contenues dans les versions des fichiers ou de la fetagents.config. Le format de ces deux fichiers est la même. Cette documentation ne fournit pas d’informations sur la façon d’écrire dans les fichiers.
  
> [!CAUTION]
> À l’aide des méthodes non prises en charge pour écrire dans les versions des fichiers ou fetagents.config peut produire des résultats inattendus, y compris les échecs du service de transport ou des agents de transport ou les deux. N’écrivez pas directement à une de ces fichiers. La méthode prise en charge uniquement pour l’écriture dans ces fichiers est en utilisant les cmdlets de l’agent de transport Exchange Management Shell. 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>Emplacement des fichiers de configuration de l’agent de transport
<a name="bk_ConfigLoc"> </a>

Lorsque vous installez Exchange 2013, le programme d’installation crée un fichier XML qui est nommé agents.config.template ou fetagents.config.template, selon le rôle de serveur est installé, dans le \<ExchangeInstallFolder\>\TransportRoles\Agents dossier (où \<ExchangeInstallFolder\> est le dossier dans lequel vous avez installé Exchange 2013). Si vous installez le rôle de serveur d’accès au Client, Exchange 2013 copie le fichier fetagents.config.template dans fetagents.config. Si vous installez le rôle serveur de boîtes aux lettres, Exchange 2013 copie le fichier agents.config.template dans les versions. Exchange 2013 lit et écrit ce fichier lorsque vous modifiez la configuration d’agents de transport sur le serveur.
  
## <a name="verifying-a-transport-agent-installation"></a>Vérifier l’installation d’un agent de transport
<a name="bk_verifyinstall"> </a>

Vous pouvez utiliser les fonctionnalités XML que le .NET Framework fournit pour lire et de valider les versions ou un fichier XML fetagents.config. Pour vérifier l’installation et la configuration d’un agent de transport, lire le code XML du fichier de configuration et recherchez l’élément de [l’agent](agent.md) qui correspond à l’agent de transport. Si un élément de **l’agent** pour l’agent de transport spécifique n’existe pas, l’agent de transport n’est pas installé. Si l’agent de transport est installé, vous pouvez lire les attributs de l’élément de **l’agent** afin de déterminer sa configuration. 
  
## <a name="configuration-file-element-hierarchy"></a>Hiérarchie d’éléments de fichier de configuration
<a name="bk_elementref"> </a>

Le code suivant montre la hiérarchie des éléments du fichier de configuration XML.
  
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
- [Concepts de l’agent d’Exchange 2013 de transport](transport-agent-concepts-in-exchange-2013.md)
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)
- [Transport des espaces de noms de l’agent dans Exchange 2013](transport-agent-namespaces-in-exchange-2013.md)
- [Cmdlets de flux de messagerie](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)
    

