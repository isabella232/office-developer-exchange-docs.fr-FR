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
# <a name="agents-configuration-file-elements-for-exchange-2013"></a><span data-ttu-id="a06fb-103">Éléments du fichier de configuration agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a06fb-103">Agents configuration file elements for Exchange 2013</span></span>

<span data-ttu-id="a06fb-104">Trouvez des informations sur les éléments XML dans le fichier de configuration fetagents.config et les versions d’Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="a06fb-104">Find information about the XML elements in the agents.config and fetagents.config configuration file in Exchange 2013.</span></span>
  
<span data-ttu-id="a06fb-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="a06fb-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="a06fb-106">Lorsque vous installez l’accès au Client ou le rôle serveur de boîtes aux lettres sur un serveur Exchange, le programme d’installation crée un fichier XML qui contient les informations de configuration des agents qui sont installés sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="a06fb-106">When you install the Client Access or the Mailbox server role on an Exchange server, the installer creates an XML file that contains configuration information about agents that are installed on the server.</span></span> <span data-ttu-id="a06fb-107">Vous ne pouvez pas écrire directement à ce fichier.</span><span class="sxs-lookup"><span data-stu-id="a06fb-107">You cannot write directly to this file.</span></span> 
  
<span data-ttu-id="a06fb-108">Le service de Transport frontal s’exécute sur des serveurs d’accès au Client et écrit dans un fichier nommé fetagents.config. Le service de Transport et le service de Transport de boîtes aux lettres s’exécutent sur des serveurs de boîtes aux lettres et écrire dans un fichier nommé versions. Un ordinateur ayant le rôle de serveur d’accès au Client et du rôle serveur de boîtes aux lettres aura à la fois un fetagents.config et un fichier de versions.</span><span class="sxs-lookup"><span data-stu-id="a06fb-108">The Front End Transport service runs on Client Access servers and writes to a file named fetagents.config. The Transport service and the Mailbox Transport service run on Mailbox servers, and write to a file named agents.config. A computer that has both the Client Access server role and the Mailbox server role will have both a fetagents.config and an agents.config file.</span></span> 
  
<span data-ttu-id="a06fb-109">Il est le seul moyen pris en charge pour écrire dans ces fichiers en utilisant les applets de commande de l’agent de transport dans Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="a06fb-109">The only supported way to write to these files is by using the transport agent cmdlets in the Exchange Management Shell.</span></span> <span data-ttu-id="a06fb-110">Pour plus d’informations sur les applets de commande de l’agent de transport, voir [Applets de commande de flux de messagerie](http://technet.microsoft.com/fr-fr/library/aa998553%28v=exchg.150%29.aspx) sur TechNet.</span><span class="sxs-lookup"><span data-stu-id="a06fb-110">For information about the transport agent cmdlets, see [Mail Flow Cmdlets](http://technet.microsoft.com/fr-fr/library/aa998553%28v=exchg.150%29.aspx) on TechNet.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a06fb-111">Pour faire la distinction entre les agents qui étendent le service de Transport frontal sur le serveur d’accès au Client et le service de Transport sur le serveur de boîtes aux lettres, cmdlets d’agent de transport ont un paramètre _TransportService_ avec la valeur « Hub » pour le Transport service et « FrontEnd » pour le service de Transport frontal.</span><span class="sxs-lookup"><span data-stu-id="a06fb-111">To distinguish between agents that extend the Front End Transport service on the Client Access server and the Transport service on the Mailbox server, transport agent cmdlets have a  _TransportService_ parameter with a value of "Hub" for the Transport service and "FrontEnd" for the Front End Transport service.</span></span> 
  
<span data-ttu-id="a06fb-112">Vous pouvez lire des versions ou fichier fetagents.config pour déterminer la présence des informations de configuration pour un ou plusieurs agents sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="a06fb-112">You can read the agents.config or fetagents.config file to determine the presence of and configuration information for one or more agents on the server.</span></span> <span data-ttu-id="a06fb-113">Cette documentation fournit une référence que vous pouvez utiliser pour lire les informations contenues dans les versions des fichiers ou de la fetagents.config. Le format de ces deux fichiers est la même.</span><span class="sxs-lookup"><span data-stu-id="a06fb-113">This documentation provides a reference that you can use to read the information in either the agents.config file or the fetagents.config. The format for both of these files is the same.</span></span> <span data-ttu-id="a06fb-114">Cette documentation ne fournit pas d’informations sur la façon d’écrire dans les fichiers.</span><span class="sxs-lookup"><span data-stu-id="a06fb-114">This documentation does not provide information about how to write to the files.</span></span>
  
> [!CAUTION]
> <span data-ttu-id="a06fb-115">À l’aide des méthodes non prises en charge pour écrire dans les versions des fichiers ou fetagents.config peut produire des résultats inattendus, y compris les échecs du service de transport ou des agents de transport ou les deux.</span><span class="sxs-lookup"><span data-stu-id="a06fb-115">Using unsupported methods to write to the agents.config file or fetagents.config can produce unexpected results, including failure of the transport service or transport agents, or both.</span></span> <span data-ttu-id="a06fb-116">N’écrivez pas directement à une de ces fichiers.</span><span class="sxs-lookup"><span data-stu-id="a06fb-116">Do not write directly to either of these files.</span></span> <span data-ttu-id="a06fb-117">La méthode prise en charge uniquement pour l’écriture dans ces fichiers est en utilisant les cmdlets de l’agent de transport Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="a06fb-117">The only supported method for writing to these files is by using the Exchange Management Shell transport agent cmdlets.</span></span> 
  
## <a name="location-of-the-transport-agent-configuration-files"></a><span data-ttu-id="a06fb-118">Emplacement des fichiers de configuration de l’agent de transport</span><span class="sxs-lookup"><span data-stu-id="a06fb-118">Location of the transport agent configuration files</span></span>
<span data-ttu-id="a06fb-119"><a name="bk_ConfigLoc"> </a></span><span class="sxs-lookup"><span data-stu-id="a06fb-119"></span></span>

<span data-ttu-id="a06fb-120">Lorsque vous installez Exchange 2013, le programme d’installation crée un fichier XML qui est nommé agents.config.template ou fetagents.config.template, selon le rôle de serveur est installé, dans le \<ExchangeInstallFolder\>\TransportRoles\Agents dossier (où \<ExchangeInstallFolder\> est le dossier dans lequel vous avez installé Exchange 2013).</span><span class="sxs-lookup"><span data-stu-id="a06fb-120">When you install Exchange 2013, the installer creates an XML file that is named either agents.config.template or fetagents.config.template, depending on the server role installed, in the \<ExchangeInstallFolder\>\TransportRoles\Agents folder (where \<ExchangeInstallFolder\> is the folder in which you installed Exchange 2013).</span></span> <span data-ttu-id="a06fb-121">Si vous installez le rôle de serveur d’accès au Client, Exchange 2013 copie le fichier fetagents.config.template dans fetagents.config. Si vous installez le rôle serveur de boîtes aux lettres, Exchange 2013 copie le fichier agents.config.template dans les versions. Exchange 2013 lit et écrit ce fichier lorsque vous modifiez la configuration d’agents de transport sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="a06fb-121">If you install the Client Access server role, Exchange 2013 copies the fetagents.config.template file to fetagents.config. If you install the Mailbox server role, Exchange 2013 copies the agents.config.template file to agents.config. Exchange 2013 reads and writes this file when you change the transport agents configuration on the server.</span></span>
  
## <a name="verifying-a-transport-agent-installation"></a><span data-ttu-id="a06fb-122">Vérifier l’installation d’un agent de transport</span><span class="sxs-lookup"><span data-stu-id="a06fb-122">Verifying a transport agent installation</span></span>
<span data-ttu-id="a06fb-123"><a name="bk_verifyinstall"> </a></span><span class="sxs-lookup"><span data-stu-id="a06fb-123"></span></span>

<span data-ttu-id="a06fb-124">Vous pouvez utiliser les fonctionnalités XML que le .NET Framework fournit pour lire et de valider les versions ou un fichier XML fetagents.config.</span><span class="sxs-lookup"><span data-stu-id="a06fb-124">You can use the XML capabilities that the .NET Framework provides to read and validate the agents.config or the fetagents.config XML file.</span></span> <span data-ttu-id="a06fb-125">Pour vérifier l’installation et la configuration d’un agent de transport, lire le code XML du fichier de configuration et recherchez l’élément de [l’agent](agent.md) qui correspond à l’agent de transport.</span><span class="sxs-lookup"><span data-stu-id="a06fb-125">To verify the installation and configuration of a transport agent, read the XML in the configuration file and find the [agent](agent.md) element that corresponds to the transport agent.</span></span> <span data-ttu-id="a06fb-126">Si un élément de **l’agent** pour l’agent de transport spécifique n’existe pas, l’agent de transport n’est pas installé.</span><span class="sxs-lookup"><span data-stu-id="a06fb-126">If an **agent** element for the specific transport agent does not exist, the transport agent is not installed.</span></span> <span data-ttu-id="a06fb-127">Si l’agent de transport est installé, vous pouvez lire les attributs de l’élément de **l’agent** afin de déterminer sa configuration.</span><span class="sxs-lookup"><span data-stu-id="a06fb-127">If the transport agent is installed, you can read the attributes of the **agent** element to determine its configuration.</span></span> 
  
## <a name="configuration-file-element-hierarchy"></a><span data-ttu-id="a06fb-128">Hiérarchie d’éléments de fichier de configuration</span><span class="sxs-lookup"><span data-stu-id="a06fb-128">Configuration file element hierarchy</span></span>
<span data-ttu-id="a06fb-129"><a name="bk_elementref"> </a></span><span class="sxs-lookup"><span data-stu-id="a06fb-129"></span></span>

<span data-ttu-id="a06fb-130">Le code suivant montre la hiérarchie des éléments du fichier de configuration XML.</span><span class="sxs-lookup"><span data-stu-id="a06fb-130">The following code shows the element hierarchy in the configuration XML file.</span></span>
  
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

## <a name="in-this-section"></a><span data-ttu-id="a06fb-131">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="a06fb-131">In this section</span></span>
<span data-ttu-id="a06fb-132"><a name="bk_elementreflist"> </a></span><span class="sxs-lookup"><span data-stu-id="a06fb-132"></span></span>

- [<span data-ttu-id="a06fb-133">agent</span><span class="sxs-lookup"><span data-stu-id="a06fb-133">agent</span></span>](agent.md)
    
- [<span data-ttu-id="a06fb-134">agentExecution</span><span class="sxs-lookup"><span data-stu-id="a06fb-134">agentExecution</span></span>](agentexecution.md)
    
- [<span data-ttu-id="a06fb-135">agentList</span><span class="sxs-lookup"><span data-stu-id="a06fb-135">agentList</span></span>](agentlist.md)
    
- [<span data-ttu-id="a06fb-136">configuration</span><span class="sxs-lookup"><span data-stu-id="a06fb-136">configuration</span></span>](configuration.md)
    
- [<span data-ttu-id="a06fb-137">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="a06fb-137">messageSnapshot</span></span>](messagesnapshot.md)
    
- [<span data-ttu-id="a06fb-138">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="a06fb-138">mexRuntime</span></span>](mexruntime.md)
    
- [<span data-ttu-id="a06fb-139">surveillance</span><span class="sxs-lookup"><span data-stu-id="a06fb-139">monitoring</span></span>](monitoring.md)
    
## <a name="see-also"></a><span data-ttu-id="a06fb-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a06fb-140">See also</span></span>

- [<span data-ttu-id="a06fb-141">Agents de transport dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a06fb-141">Transport agents in Exchange</span></span>](transport-agents-in-exchange-2013.md)
- [<span data-ttu-id="a06fb-142">Concepts de l’agent d’Exchange 2013 de transport</span><span class="sxs-lookup"><span data-stu-id="a06fb-142">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="a06fb-143">Référence de l’agent de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a06fb-143">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
- [<span data-ttu-id="a06fb-144">Transport des espaces de noms de l’agent dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a06fb-144">Transport agent namespaces in Exchange 2013</span></span>](transport-agent-namespaces-in-exchange-2013.md)
- [<span data-ttu-id="a06fb-145">Cmdlets de flux de messagerie</span><span class="sxs-lookup"><span data-stu-id="a06fb-145">Mail Flow Cmdlets</span></span>](https://docs.microsoft.com/fr-fr/powershell/exchange/?view=exchange-ps)
    

