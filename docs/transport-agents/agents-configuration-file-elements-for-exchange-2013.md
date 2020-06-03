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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461568"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a><span data-ttu-id="8bb85-103">Éléments du fichier de configuration des agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8bb85-103">Agents configuration file elements for Exchange 2013</span></span>

<span data-ttu-id="8bb85-104">Recherchez des informations sur les éléments XML dans le fichier de configuration agents. config et fetagents. config dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="8bb85-104">Find information about the XML elements in the agents.config and fetagents.config configuration file in Exchange 2013.</span></span>
  
<span data-ttu-id="8bb85-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="8bb85-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="8bb85-106">Lorsque vous installez le rôle serveur d’accès au client ou de boîte aux lettres sur un serveur Exchange, le programme d’installation crée un fichier XML qui contient des informations de configuration sur les agents installés sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="8bb85-106">When you install the Client Access or the Mailbox server role on an Exchange server, the installer creates an XML file that contains configuration information about agents that are installed on the server.</span></span> <span data-ttu-id="8bb85-107">Vous ne pouvez pas écrire directement dans ce fichier.</span><span class="sxs-lookup"><span data-stu-id="8bb85-107">You cannot write directly to this file.</span></span> 
  
<span data-ttu-id="8bb85-108">Le service de transport frontal s’exécute sur les serveurs d’accès au client et écrit dans un fichier nommé fetagents. config. Le service de transport et le service de transport de boîtes aux lettres s’exécutent sur des serveurs de boîtes aux lettres, et sont écrits dans un fichier nommé agents. config. Un ordinateur qui a à la fois le rôle serveur d’accès au client et le rôle serveur de boîte aux lettres aura à la fois un fichier fetagents. config et un fichier agents. config.</span><span class="sxs-lookup"><span data-stu-id="8bb85-108">The Front End Transport service runs on Client Access servers and writes to a file named fetagents.config. The Transport service and the Mailbox Transport service run on Mailbox servers, and write to a file named agents.config. A computer that has both the Client Access server role and the Mailbox server role will have both a fetagents.config and an agents.config file.</span></span> 
  
<span data-ttu-id="8bb85-109">La seule façon d’écrire dans ces fichiers est d’utiliser les applets de commande de l’agent de transport dans l’environnement de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="8bb85-109">The only supported way to write to these files is by using the transport agent cmdlets in the Exchange Management Shell.</span></span> <span data-ttu-id="8bb85-110">Pour plus d’informations sur les applets de commande de l’agent de transport, consultez la rubrique [mail Flow cmdlets](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) on technet.</span><span class="sxs-lookup"><span data-stu-id="8bb85-110">For information about the transport agent cmdlets, see [Mail Flow Cmdlets](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) on TechNet.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="8bb85-111">Pour faire la distinction entre les agents qui étendent le service de transport frontal sur le serveur d’accès au client et le service de transport sur le serveur de boîtes aux lettres, les cmdlets de l’agent de transport ont un paramètre _TransportService_ avec la valeur « Hub » pour le service de transport et « frontend » pour le service de transport frontal.</span><span class="sxs-lookup"><span data-stu-id="8bb85-111">To distinguish between agents that extend the Front End Transport service on the Client Access server and the Transport service on the Mailbox server, transport agent cmdlets have a  _TransportService_ parameter with a value of "Hub" for the Transport service and "FrontEnd" for the Front End Transport service.</span></span> 
  
<span data-ttu-id="8bb85-112">Vous pouvez lire le fichier agents. config ou fetagents. config pour déterminer la présence et les informations de configuration d’un ou de plusieurs agents sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="8bb85-112">You can read the agents.config or fetagents.config file to determine the presence of and configuration information for one or more agents on the server.</span></span> <span data-ttu-id="8bb85-113">Cette documentation fournit une référence que vous pouvez utiliser pour lire les informations dans le fichier agents. config ou fetagents. config. Le format de ces deux fichiers est le même.</span><span class="sxs-lookup"><span data-stu-id="8bb85-113">This documentation provides a reference that you can use to read the information in either the agents.config file or the fetagents.config. The format for both of these files is the same.</span></span> <span data-ttu-id="8bb85-114">Cette documentation ne fournit pas d’informations sur la façon d’écrire dans les fichiers.</span><span class="sxs-lookup"><span data-stu-id="8bb85-114">This documentation does not provide information about how to write to the files.</span></span>
  
> [!CAUTION]
> <span data-ttu-id="8bb85-115">L’utilisation de méthodes non prises en charge pour écrire dans le fichier agents. config ou fetagents. config peut produire des résultats inattendus, notamment l’échec du service de transport ou des agents de transport, ou les deux.</span><span class="sxs-lookup"><span data-stu-id="8bb85-115">Using unsupported methods to write to the agents.config file or fetagents.config can produce unexpected results, including failure of the transport service or transport agents, or both.</span></span> <span data-ttu-id="8bb85-116">N’écrivez pas directement dans l’un de ces fichiers.</span><span class="sxs-lookup"><span data-stu-id="8bb85-116">Do not write directly to either of these files.</span></span> <span data-ttu-id="8bb85-117">La seule méthode prise en charge pour l’écriture dans ces fichiers est d’utiliser les cmdlets de l’agent de transport de l’environnement de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="8bb85-117">The only supported method for writing to these files is by using the Exchange Management Shell transport agent cmdlets.</span></span> 
  
## <a name="location-of-the-transport-agent-configuration-files"></a><span data-ttu-id="8bb85-118">Emplacement des fichiers de configuration de l’agent de transport</span><span class="sxs-lookup"><span data-stu-id="8bb85-118">Location of the transport agent configuration files</span></span>
<span data-ttu-id="8bb85-119"><a name="bk_ConfigLoc"> </a></span><span class="sxs-lookup"><span data-stu-id="8bb85-119"><a name="bk_ConfigLoc"> </a></span></span>

<span data-ttu-id="8bb85-120">Lorsque vous installez Exchange 2013, le programme d’installation crée un fichier XML nommé agents. config. template ou fetagents. config. Template, selon le rôle serveur installé, dans le \<ExchangeInstallFolder\> dossier \TransportRoles\Agents (où \<ExchangeInstallFolder\> est le dossier dans lequel vous avez installé Exchange 2013).</span><span class="sxs-lookup"><span data-stu-id="8bb85-120">When you install Exchange 2013, the installer creates an XML file that is named either agents.config.template or fetagents.config.template, depending on the server role installed, in the \<ExchangeInstallFolder\>\TransportRoles\Agents folder (where \<ExchangeInstallFolder\> is the folder in which you installed Exchange 2013).</span></span> <span data-ttu-id="8bb85-121">Si vous installez le rôle serveur d’accès au client, Exchange 2013 copie le fichier fetagents. config. template dans fetagents. config. Si vous installez le rôle serveur de boîtes aux lettres, Exchange 2013 copie le fichier agents. config. template dans agents. config. Exchange 2013 lit et écrit ce fichier lorsque vous modifiez la configuration des agents de transport sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="8bb85-121">If you install the Client Access server role, Exchange 2013 copies the fetagents.config.template file to fetagents.config. If you install the Mailbox server role, Exchange 2013 copies the agents.config.template file to agents.config. Exchange 2013 reads and writes this file when you change the transport agents configuration on the server.</span></span>
  
## <a name="verifying-a-transport-agent-installation"></a><span data-ttu-id="8bb85-122">Vérification de l’installation d’un agent de transport</span><span class="sxs-lookup"><span data-stu-id="8bb85-122">Verifying a transport agent installation</span></span>
<span data-ttu-id="8bb85-123"><a name="bk_verifyinstall"> </a></span><span class="sxs-lookup"><span data-stu-id="8bb85-123"><a name="bk_verifyinstall"> </a></span></span>

<span data-ttu-id="8bb85-124">Vous pouvez utiliser les fonctionnalités XML fournies par .NET Framework pour lire et valider le fichier agents. config ou le fichier XML fetagents. config.</span><span class="sxs-lookup"><span data-stu-id="8bb85-124">You can use the XML capabilities that the .NET Framework provides to read and validate the agents.config or the fetagents.config XML file.</span></span> <span data-ttu-id="8bb85-125">Pour vérifier l’installation et la configuration d’un agent de transport, lisez le code XML dans le fichier de configuration et recherchez l’élément [agent](agent.md) correspondant à l’agent de transport.</span><span class="sxs-lookup"><span data-stu-id="8bb85-125">To verify the installation and configuration of a transport agent, read the XML in the configuration file and find the [agent](agent.md) element that corresponds to the transport agent.</span></span> <span data-ttu-id="8bb85-126">Si un élément **agent** pour l’agent de transport spécifique n’existe pas, l’agent de transport n’est pas installé.</span><span class="sxs-lookup"><span data-stu-id="8bb85-126">If an **agent** element for the specific transport agent does not exist, the transport agent is not installed.</span></span> <span data-ttu-id="8bb85-127">Si l’agent de transport est installé, vous pouvez lire les attributs de l’élément **agent** pour en déterminer la configuration.</span><span class="sxs-lookup"><span data-stu-id="8bb85-127">If the transport agent is installed, you can read the attributes of the **agent** element to determine its configuration.</span></span> 
  
## <a name="configuration-file-element-hierarchy"></a><span data-ttu-id="8bb85-128">Hiérarchie des éléments du fichier de configuration</span><span class="sxs-lookup"><span data-stu-id="8bb85-128">Configuration file element hierarchy</span></span>
<span data-ttu-id="8bb85-129"><a name="bk_elementref"> </a></span><span class="sxs-lookup"><span data-stu-id="8bb85-129"><a name="bk_elementref"> </a></span></span>

<span data-ttu-id="8bb85-130">Le code suivant montre la hiérarchie des éléments dans le fichier XML de configuration.</span><span class="sxs-lookup"><span data-stu-id="8bb85-130">The following code shows the element hierarchy in the configuration XML file.</span></span>
  
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

## <a name="in-this-section"></a><span data-ttu-id="8bb85-131">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="8bb85-131">In this section</span></span>
<span data-ttu-id="8bb85-132"><a name="bk_elementreflist"> </a></span><span class="sxs-lookup"><span data-stu-id="8bb85-132"><a name="bk_elementreflist"> </a></span></span>

- [<span data-ttu-id="8bb85-133">agent</span><span class="sxs-lookup"><span data-stu-id="8bb85-133">agent</span></span>](agent.md)
    
- [<span data-ttu-id="8bb85-134">agentExecution</span><span class="sxs-lookup"><span data-stu-id="8bb85-134">agentExecution</span></span>](agentexecution.md)
    
- [<span data-ttu-id="8bb85-135">agentList</span><span class="sxs-lookup"><span data-stu-id="8bb85-135">agentList</span></span>](agentlist.md)
    
- [<span data-ttu-id="8bb85-136">configuration</span><span class="sxs-lookup"><span data-stu-id="8bb85-136">configuration</span></span>](configuration.md)
    
- [<span data-ttu-id="8bb85-137">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="8bb85-137">messageSnapshot</span></span>](messagesnapshot.md)
    
- [<span data-ttu-id="8bb85-138">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="8bb85-138">mexRuntime</span></span>](mexruntime.md)
    
- [<span data-ttu-id="8bb85-139">surveillance</span><span class="sxs-lookup"><span data-stu-id="8bb85-139">monitoring</span></span>](monitoring.md)
    
## <a name="see-also"></a><span data-ttu-id="8bb85-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8bb85-140">See also</span></span>

- [<span data-ttu-id="8bb85-141">Agents de transport dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8bb85-141">Transport agents in Exchange</span></span>](transport-agents-in-exchange-2013.md)
- [<span data-ttu-id="8bb85-142">Concepts sur les agents de transport dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8bb85-142">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="8bb85-143">Référence de l’agent de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8bb85-143">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
- [<span data-ttu-id="8bb85-144">Espaces de noms de l’agent de transport dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8bb85-144">Transport agent namespaces in Exchange 2013</span></span>](transport-agent-namespaces-in-exchange-2013.md)
- [<span data-ttu-id="8bb85-145">Cmdlets de flux de messagerie</span><span class="sxs-lookup"><span data-stu-id="8bb85-145">Mail Flow Cmdlets</span></span>](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

