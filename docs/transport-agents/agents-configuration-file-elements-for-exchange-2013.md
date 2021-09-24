---
title: Éléments de fichier de configuration des agents Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Agents
api_type:
- schema
ms.assetid: 3047653b-d712-46c1-ae0a-73f3975f5e9d
description: Trouvez des informations sur les éléments XML dans le fichier de configuration agents.config et fetagents.config dans Exchange 2013.
ms.openlocfilehash: bdf394130f7818c5b956e8b15eed86a6318b9698
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510420"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Éléments de fichier de configuration des agents Exchange 2013

Trouvez des informations sur les éléments XML dans le fichier de configuration agents.config et fetagents.config dans Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Lorsque vous installez le rôle serveur d’accès au client ou de boîtes aux lettres sur un serveur Exchange, le programme d’installation crée un fichier XML qui contient des informations de configuration sur les agents installés sur le serveur. Vous ne pouvez pas écrire directement dans ce fichier. 
  
Le service de transport frontal s’exécute sur les serveurs d’accès au client et écrit dans un fichier nommé fetagents.config. Le service de transport et le service de transport de boîtes aux lettres s’exécutent sur des serveurs de boîtes aux lettres et écrivent dans un fichier nommé agents.config. Un ordinateur qui possède à la fois le rôle serveur d’accès au client et le rôle serveur de boîtes aux lettres dispose d’un fetagents.config et d’un agents.config'accès au client. 
  
La seule façon d’écrire dans ces fichiers est d’utiliser les cmdlets d’agent de transport dans Exchange Management Shell. Pour plus d’informations sur les cmdlets d’agent de transport, voir [Mail Flow Cmdlets](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) sur TechNet. 
  
> [!NOTE]
> Pour faire la distinction entre les agents qui étendent le service de transport frontal sur le serveur d’accès au client et le service de transport sur le serveur de boîtes aux lettres, les cmdlets d’agent de transport ont un paramètre  _TransportService_ avec la valeur « Hub » pour le service de transport et « FrontEnd » pour le service de transport frontal. 
  
Vous pouvez lire le fichier agents.config ou fetagents.config pour déterminer la présence et les informations de configuration d’un ou plusieurs agents sur le serveur. Cette documentation fournit une référence que vous pouvez utiliser pour lire les informations dans le fichier agents.config ou le fetagents.config. Le format de ces deux fichiers est le même. Cette documentation ne fournit pas d’informations sur la façon d’écrire dans les fichiers.
  
> [!CAUTION]
> L’utilisation de méthodes non pris en agents.config pour écrire dans le fichier ou le fetagents.config agents.config peut produire des résultats inattendus, notamment l’échec du service de transport ou des agents de transport, ou les deux. N’écrivez pas directement dans l’un de ces fichiers. La seule méthode prise en charge pour écrire dans ces fichiers est l’utilisation des cmdlets d’agent de transport Exchange Management Shell. 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>Emplacement des fichiers de configuration de l’agent de transport
<a name="bk_ConfigLoc"> </a>

Lorsque vous installez Exchange 2013, le programme d’installation crée un fichier XML nommé agents.config.template ou fetagents.config.template, selon le rôle serveur installé, dans le dossier \TransportRoles\Agents (où se trouve le dossier dans lequel vous avez installé \<ExchangeInstallFolder\> \<ExchangeInstallFolder\> Exchange 2013). Si vous installez le rôle serveur d’accès au client, Exchange 2013 copie le fichier fetagents.config.template dans fetagents.config. Si vous installez le rôle serveur de boîtes aux lettres, Exchange 2013 copie le fichier agents.config.template vers agents.config. Exchange 2013 lit et écrit ce fichier lorsque vous modifiez la configuration des agents de transport sur le serveur.
  
## <a name="verifying-a-transport-agent-installation"></a>Vérification de l’installation d’un agent de transport
<a name="bk_verifyinstall"> </a>

Vous pouvez utiliser les fonctionnalités XML que le .NET Framework fournit pour lire et valider le fichier agents.config ou le fichier XML fetagents.config de données. Pour vérifier l’installation et la configuration d’un agent de transport, lisez le XML dans le fichier de configuration et recherchez l’élément [agent](agent.md) qui correspond à l’agent de transport. Si aucun **élément agent** n’existe pour l’agent de transport spécifique, l’agent de transport n’est pas installé. Si l’agent de transport est installé, vous pouvez lire les attributs de l’élément **agent** pour déterminer sa configuration. 
  
## <a name="configuration-file-element-hierarchy"></a>Hiérarchie des éléments de fichier de configuration
<a name="bk_elementref"> </a>

Le code suivant montre la hiérarchie d’éléments dans le fichier XML de configuration.
  
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
- [Référence de l’agent de transport Exchange 2013](transport-agent-reference-for-exchange-2013.md)
- [Espaces de noms d’agent de transport Exchange 2013](transport-agent-namespaces-in-exchange-2013.md)
- [Cmdlets Flow messagerie](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

