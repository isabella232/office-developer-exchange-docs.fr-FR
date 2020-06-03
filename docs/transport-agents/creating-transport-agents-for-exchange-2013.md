---
title: Création d’agents de transport pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Trouvez des informations sur la création d’agents de transport personnalisés pour Exchange 2013 et sur la configuration système requise pour la création d’un agent personnalisé.
ms.openlocfilehash: cb1cd180817524fe29a100a48d90444c75a77510
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462373"
---
# <a name="creating-transport-agents-for-exchange-2013"></a><span data-ttu-id="a408b-103">Création d’agents de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a408b-103">Creating transport agents for Exchange 2013</span></span>

<span data-ttu-id="a408b-104">Trouvez des informations sur la création d’agents de transport personnalisés pour Exchange 2013 et sur la configuration système requise pour la création d’un agent personnalisé.</span><span class="sxs-lookup"><span data-stu-id="a408b-104">Find information about how to create custom transport agents for Exchange 2013, and the system requirements for creating a custom agent.</span></span>
  
<span data-ttu-id="a408b-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="a408b-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="a408b-106">Exchange Server 2013 comprend plusieurs agents de transport que vous pouvez utiliser pour traiter les messages.</span><span class="sxs-lookup"><span data-stu-id="a408b-106">Exchange Server 2013 includes several transport agents that you can use to process messages.</span></span> <span data-ttu-id="a408b-107">À l’aide des assemblys inclus dans Exchange, vous pouvez créer vos propres agents personnalisés pour effectuer des tâches spécifiques en fonction des besoins de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="a408b-107">By using the assemblies that come with Exchange, you can create your own custom agents to perform specific tasks according to the needs of your organization.</span></span> <span data-ttu-id="a408b-108">Par exemple, vous pouvez utiliser un agent de transport SmtpReceiveAgent pour intercepter les messages reçus via le protocole SMTP et traiter le message pour convertir le format du corps afin qu’il contienne du texte préformaté.</span><span class="sxs-lookup"><span data-stu-id="a408b-108">For example, you can use an SmtpReceiveAgent transport agent to intercept messages that are received via the SMTP protocol and process the message to convert the format of the body to contain preformatted text.</span></span> <span data-ttu-id="a408b-109">Vous pouvez utiliser un agent de transport RoutingAgent pour consigner les messages qui transitent par le serveur sur un autre serveur.</span><span class="sxs-lookup"><span data-stu-id="a408b-109">You can use a RoutingAgent transport agent to log the messages that pass through the server on route to another server.</span></span> <span data-ttu-id="a408b-110">Vous pouvez également créer des fonctionnalités plus complexes qui utilisent plusieurs types d’agents.</span><span class="sxs-lookup"><span data-stu-id="a408b-110">You can also create more complex features that make use of more than one type of agent.</span></span> <span data-ttu-id="a408b-111">Par exemple, pour créer un agent antivirus, vous pouvez implémenter un SmtpReceiveAgent et un agent RoutingAgent.</span><span class="sxs-lookup"><span data-stu-id="a408b-111">For example, to create an antivirus agent, you can implement an SmtpReceiveAgent and a RoutingAgent agent.</span></span> <span data-ttu-id="a408b-112">Si votre réseau comporte un composant qui ne prend pas en charge le protocole SMTP, vous pouvez utiliser un agent de transport DeliveryAgent pour gérer la communication entre votre serveur Exchange et votre composant externe.</span><span class="sxs-lookup"><span data-stu-id="a408b-112">If you have a component on your network that does not support the SMTP protocol, you can use a DeliveryAgent transport agent to handle the communication between your Exchange server and your external component.</span></span> 
  
<span data-ttu-id="a408b-113">Cet article fournit des informations sur les conditions préalables et les tâches impliquées dans la création de votre propre agent de transport.</span><span class="sxs-lookup"><span data-stu-id="a408b-113">This article provides information about the prerequisites for and tasks involved in creating your own transport agent.</span></span> <span data-ttu-id="a408b-114">Pour plus d’informations sur la création d’agents de transport spécifiques, consultez [la rubrique Create a RoutingAgent transport agent for exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create a SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)et [Create a DeliveryAgent transport agent for Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="a408b-114">For information about creating specific transport agents, see [Create a RoutingAgent transport agent for Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create an SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), and [Create a DeliveryAgent transport agent for Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span></span>
  
## <a name="prerequisites-for-creating-a-transport-agent"></a><span data-ttu-id="a408b-115">Conditions préalables à la création d’un agent de transport</span><span class="sxs-lookup"><span data-stu-id="a408b-115">Prerequisites for creating a transport agent</span></span>
<span data-ttu-id="a408b-116"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="a408b-116"><a name="bk_prerequisites"> </a></span></span>

<span data-ttu-id="a408b-117">Les conditions préalables requises pour implémenter un agent de transport sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="a408b-117">The following are the prerequisites that you need in order to implement a transport agent:</span></span>
  
- <span data-ttu-id="a408b-118">Un ordinateur exécutant Exchange 2013 qui exécute le service de transport frontal sur un serveur d’accès au client ou de transport Edge, ou le service de transport sur un serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a408b-118">A computer running Exchange 2013 that is running the Front End Transport service on a Client Access or Edge Transport server, or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="a408b-119">Pour plus d’informations sur l’architecture des rôles serveur dans Exchange 2013, voir [transport agent concepts in exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="a408b-119">For information about the server role architecture in Exchange 2013, see [Transport agent concepts in Exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span></span>
    
- <span data-ttu-id="a408b-120">Les assemblys suivants pour les classes d’agent de transport :</span><span class="sxs-lookup"><span data-stu-id="a408b-120">The following assemblies for the transport agent classes:</span></span>
    
  - <span data-ttu-id="a408b-121">Microsoft. Exchange. Data. dll</span><span class="sxs-lookup"><span data-stu-id="a408b-121">Microsoft.Exchange.Data.dll</span></span>
    
  - <span data-ttu-id="a408b-122">Microsoft. Exchange. Data. Common. dll</span><span class="sxs-lookup"><span data-stu-id="a408b-122">Microsoft.Exchange.Data.Common.dll</span></span>
    
  - <span data-ttu-id="a408b-123">Microsoft. Exchange. transport. dll</span><span class="sxs-lookup"><span data-stu-id="a408b-123">Microsoft.Exchange.Transport.dll</span></span>
    
- <span data-ttu-id="a408b-124">.NET Framework 4,5</span><span class="sxs-lookup"><span data-stu-id="a408b-124">The .NET Framework 4.5</span></span>
    
<span data-ttu-id="a408b-125">Nous vous recommandons également d’installer Visual Studio 2012.</span><span class="sxs-lookup"><span data-stu-id="a408b-125">We also recommend that you install Visual Studio 2012.</span></span> <span data-ttu-id="a408b-126">Vous pouvez implémenter des agents de transport à l’aide de Visual Basic .NET ou C#.</span><span class="sxs-lookup"><span data-stu-id="a408b-126">You can implement transport agents by using either Visual Basic .NET or C#.</span></span>
  
## <a name="referencing-the-assemblies"></a><span data-ttu-id="a408b-127">Référencement des assemblys</span><span class="sxs-lookup"><span data-stu-id="a408b-127">Referencing the assemblies</span></span>
<span data-ttu-id="a408b-128"><a name="bk_ReferenceAssemblies"> </a></span><span class="sxs-lookup"><span data-stu-id="a408b-128"><a name="bk_ReferenceAssemblies"> </a></span></span>

<span data-ttu-id="a408b-129">Exchange 2013 fournit une bibliothèque de classes qui prennent en charge l’extension du comportement de transport Exchange.</span><span class="sxs-lookup"><span data-stu-id="a408b-129">Exchange 2013 provides a library of classes that support the extension of Exchange transport behavior.</span></span> <span data-ttu-id="a408b-130">Ces classes requièrent .NET Framework 4,5.</span><span class="sxs-lookup"><span data-stu-id="a408b-130">These classes require the .NET Framework 4.5.</span></span> <span data-ttu-id="a408b-131">Vous pouvez implémenter des agents de transport basés sur ces classes à l’aide de Visual Studio 2012.</span><span class="sxs-lookup"><span data-stu-id="a408b-131">You can implement transport agents based on these classes by using Visual Studio 2012.</span></span>
  
<span data-ttu-id="a408b-132">Le programme d’installation d’Exchange 2013 installe les assemblys qui sont utilisés pour le développement de l’agent de transport et les enregistre dans le global assembly cache (GAC).</span><span class="sxs-lookup"><span data-stu-id="a408b-132">The Exchange 2013 installer installs assemblies that are used for transport agent development and registers them in the global assembly cache (GAC).</span></span> <span data-ttu-id="a408b-133">Pour commencer à implémenter un agent de transport, créez une référence à l’assembly Microsoft. Exchange. Data. transport dans un projet de bibliothèque de classes.</span><span class="sxs-lookup"><span data-stu-id="a408b-133">To begin implementing a transport agent, create a reference to the Microsoft.Exchange.Data.Transport assembly in a class library project.</span></span>
  
## <a name="implementing-a-transport-agent"></a><span data-ttu-id="a408b-134">Implémentation d’un agent de transport</span><span class="sxs-lookup"><span data-stu-id="a408b-134">Implementing a transport agent</span></span>
<span data-ttu-id="a408b-135"><a name="bk_implementationExample"> </a></span><span class="sxs-lookup"><span data-stu-id="a408b-135"><a name="bk_implementationExample"> </a></span></span>

<span data-ttu-id="a408b-136">L’exemple suivant montre une implémentation minimale de classes qui dérivent des classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a408b-136">The following example shows a minimal implementation of classes that derive from the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="a408b-137">Si plusieurs agents de transport sont installés et inscrits pour le même événement, tous les agents sont appelés, même si un agent supprime tous les destinataires d’un élément de courrier.</span><span class="sxs-lookup"><span data-stu-id="a408b-137">If multiple transport agents are installed and registered for the same event, all agents will be invoked, even if one agent removes all the recipients from a mail item.</span></span> <span data-ttu-id="a408b-138">> pour éviter les erreurs non gérées ou les comportements imprévisibles, votre agent de transport doit gérer les cas dans lesquels le nombre de destinataires d’un élément de courrier est égal à zéro.</span><span class="sxs-lookup"><span data-stu-id="a408b-138">> To avoid unhandled errors or unpredictable behavior, your transport agent should handle cases in which the recipient count on a mail item is equal to zero.</span></span> 
  
```cs
using System;
using System.Collections.Generic;
using System.Text;
using Microsoft.Exchange.Data.Transport;
using Microsoft.Exchange.Data.Transport.Smtp;
namespace MyAgents
{
    public sealed class MyAgentFactory : SmtpReceiveAgentFactory
    {
        public override SmtpReceiveAgent CreateAgent(SmtpServer server)
        {
            return new MyAgent();
        }
    }
    public class MyAgent : SmtpReceiveAgent
    {
        public MyAgent()
        {
            this.OnEndOfData += new EndOfDataEventHandler(MyEndOfDataHandler);
        }
        private void MyEndOfDataHandler (ReceiveMessageEventSource source, EndOfDataEventArgs e)
        {
            // The following line appends text to the subject of the message that caused the event.
            e.MailItem.Message.Subject += " - this text appended by MyAgent";
        }
    }
}
```

```vb
Imports System
Imports System.Collections.Generic
Imports System.Text
Imports Microsoft.Exchange.Data.Transport
Imports Microsoft.Exchange.Data.Transport.Smtp
Namespace MyAgents
    NotInheritable Class MyAgentFactory
        Inherits SmtpReceiveAgentFactory
        Public Overrides Function CreateAgent(ByVal server as SmtpServer) As SmtpReceiveAgent
            Return New MyAgent
        End Function
    End Class
    Public Class MyAgent
        Inherits SmtpReceiveAgent
        Private Sub MyEndOfDataHandler(ByVal source As ReceiveMessageEventSource, ByVal e As EndOfDataEventArgs) Handles Me.OnEndOfData
            ' The following line appends text to the subject of the message that caused the event.
            e.MailItem.Message.Subject &amp;= e.MailItem.Message.Subject + " - this text appended by MyAgent"
        End Sub
    End Class
End Namespace
```

## <a name="installing-and-enabling-an-agent"></a><span data-ttu-id="a408b-139">Installation et activation d’un agent</span><span class="sxs-lookup"><span data-stu-id="a408b-139">Installing and enabling an agent</span></span>
<span data-ttu-id="a408b-140"><a name="bk_InstallEnable"> </a></span><span class="sxs-lookup"><span data-stu-id="a408b-140"><a name="bk_InstallEnable"> </a></span></span>

<span data-ttu-id="a408b-141">Une fois que vous avez compilé votre agent sur une DLL, vous devez installer et activer l’agent sur votre serveur Exchange de développement.</span><span class="sxs-lookup"><span data-stu-id="a408b-141">After you compile your agent to a DLL, you must install and enable the agent on your development Exchange server.</span></span> <span data-ttu-id="a408b-142">Dans l’environnement de commande Exchange Management Shell, utilisez l’applet de commande [install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) pour installer votre agent et la cmdlet [Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx) pour activer votre agent.</span><span class="sxs-lookup"><span data-stu-id="a408b-142">In the Exchange Management Shell, use the [Install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) cmdlet to install your agent, and the [Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx) cmdlet to enable your agent.</span></span> <span data-ttu-id="a408b-143">Pour plus d’informations sur l’utilisation de l’environnement de commande Exchange Management Shell, consultez la rubrique [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="a408b-143">For information about how to use the Exchange Management Shell, see [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span></span>
  
> [!CAUTION]
> <span data-ttu-id="a408b-144">Les agents de transport ont un accès illimité aux messages électroniques qu'ils rencontrent.</span><span class="sxs-lookup"><span data-stu-id="a408b-144">Transport agents have full access to all email messages that they encounter.</span></span> <span data-ttu-id="a408b-145">Exchange 2013 ne limite pas le comportement d’un agent de transport.</span><span class="sxs-lookup"><span data-stu-id="a408b-145">Exchange 2013 does not restrict the behavior of a transport agent.</span></span> <span data-ttu-id="a408b-146">Les agents de transport instables ou qui contiennent des failles de sécurité peuvent affecter la stabilité et la sécurité d’Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="a408b-146">Transport agents that are unstable or that contain security flaws might affect the stability and security of Exchange 2013.</span></span> <span data-ttu-id="a408b-147">Par conséquent, vous devez uniquement installer des agents de transport dont vous avez entièrement confiance et qui ont été entièrement testés.</span><span class="sxs-lookup"><span data-stu-id="a408b-147">Therefore, you should only install transport agents that you fully trust and that have been fully tested.</span></span> 
  
<span data-ttu-id="a408b-148">Lorsque vous utilisez la cmdlet **install-TransportAgent** pour installer un agent, l’environnement de commande Exchange Management Shell conserve un verrou sur l’assembly.</span><span class="sxs-lookup"><span data-stu-id="a408b-148">When you use the **Install-TransportAgent** cmdlet to install an agent, the Exchange Management Shell keeps a lock on the assembly.</span></span> <span data-ttu-id="a408b-149">Pour libérer le verrou sur l’assembly, vous devez fermer l’instance de l’environnement de commande Exchange Management Shell que vous avez utilisée pour installer l’agent.</span><span class="sxs-lookup"><span data-stu-id="a408b-149">To release the lock on the assembly, you must close the instance of the Exchange Management Shell that you used to install the agent.</span></span> <span data-ttu-id="a408b-150">Vous ne pourrez pas mettre à jour l’assembly tant que vous n’aurez pas libéré le verrou.</span><span class="sxs-lookup"><span data-stu-id="a408b-150">You will be unable to update the assembly until you release the lock.</span></span> 
  
<span data-ttu-id="a408b-151">L’exemple suivant montre comment utiliser l’environnement de commande Exchange Management Shell pour installer et activer un agent nommé MyAgent à l’aide d’une classe dérivée de [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) nommée MyAgents. MyAgentFactory.</span><span class="sxs-lookup"><span data-stu-id="a408b-151">The following example shows how to use the Exchange Management Shell to install and enable an agent named MyAgent by using a class derived from [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) named MyAgents.MyAgentFactory.</span></span> 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
<span data-ttu-id="a408b-152">Cet exemple nomme l’agent MyCustomAgent sur le serveur sur lequel l’agent est installé.</span><span class="sxs-lookup"><span data-stu-id="a408b-152">This example names the agent MyCustomAgent on the server on which the agent is installed.</span></span> <span data-ttu-id="a408b-153">L’exemple suivant montre comment activer l’agent nommé MyCustomAgent.</span><span class="sxs-lookup"><span data-stu-id="a408b-153">The following example shows how to enable the agent named MyCustomAgent.</span></span>
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
<span data-ttu-id="a408b-154">Pour gérer un agent de transport dans le service de transport frontal sur un serveur d’accès au client, ajoutez la valeur suivante à la commande : `-TransportService FrontEnd` .</span><span class="sxs-lookup"><span data-stu-id="a408b-154">To manage a transport agent in the Front End Transport service on a Client Access server, add the following value to the command:  `-TransportService FrontEnd`.</span></span> <span data-ttu-id="a408b-155">Par exemple, pour afficher les agents de transport dans le service de transport frontal, exécutez la commande suivante.</span><span class="sxs-lookup"><span data-stu-id="a408b-155">For example, to view the transport agents in the Front End Transport service, run the following command.</span></span>
  
 `Get-TransportAgent -TransportService FrontEnd`
  
<span data-ttu-id="a408b-156">Pour plus d’informations sur l’installation, l’activation et la gestion de votre agent, voir [gérer les agents de transport](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="a408b-156">For more information about installing, enabling, and managing your agent, see [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="a408b-157">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="a408b-157">In this section</span></span>
<span data-ttu-id="a408b-158"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="a408b-158"><a name="bk_inthissection"> </a></span></span>

- [<span data-ttu-id="a408b-159">Création d’un agent de transport RoutingAgent pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a408b-159">Create a RoutingAgent transport agent for Exchange 2013</span></span>](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="a408b-160">Création d’un agent de transport SmtpReceiveAgent pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a408b-160">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="a408b-161">Création d’un agent de transport DeliveryAgent pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a408b-161">Create a DeliveryAgent transport agent for Exchange 2013</span></span>](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="a408b-162">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a408b-162">See also</span></span>

- [<span data-ttu-id="a408b-163">Concepts sur les agents de transport dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a408b-163">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)   
- [<span data-ttu-id="a408b-164">Référence de l’agent de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a408b-164">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    

