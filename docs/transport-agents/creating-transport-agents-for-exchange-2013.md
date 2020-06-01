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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462373"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Création d’agents de transport pour Exchange 2013

Trouvez des informations sur la création d’agents de transport personnalisés pour Exchange 2013 et sur la configuration système requise pour la création d’un agent personnalisé.
  
**S’applique à :** Exchange Server 2013
  
Exchange Server 2013 comprend plusieurs agents de transport que vous pouvez utiliser pour traiter les messages. À l’aide des assemblys inclus dans Exchange, vous pouvez créer vos propres agents personnalisés pour effectuer des tâches spécifiques en fonction des besoins de votre organisation. Par exemple, vous pouvez utiliser un agent de transport SmtpReceiveAgent pour intercepter les messages reçus via le protocole SMTP et traiter le message pour convertir le format du corps afin qu’il contienne du texte préformaté. Vous pouvez utiliser un agent de transport RoutingAgent pour consigner les messages qui transitent par le serveur sur un autre serveur. Vous pouvez également créer des fonctionnalités plus complexes qui utilisent plusieurs types d’agents. Par exemple, pour créer un agent antivirus, vous pouvez implémenter un SmtpReceiveAgent et un agent RoutingAgent. Si votre réseau comporte un composant qui ne prend pas en charge le protocole SMTP, vous pouvez utiliser un agent de transport DeliveryAgent pour gérer la communication entre votre serveur Exchange et votre composant externe. 
  
Cet article fournit des informations sur les conditions préalables et les tâches impliquées dans la création de votre propre agent de transport. Pour plus d’informations sur la création d’agents de transport spécifiques, consultez [la rubrique Create a RoutingAgent transport agent for exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create a SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)et [Create a DeliveryAgent transport agent for Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>Conditions préalables à la création d’un agent de transport
<a name="bk_prerequisites"> </a>

Les conditions préalables requises pour implémenter un agent de transport sont les suivantes :
  
- Un ordinateur exécutant Exchange 2013 qui exécute le service de transport frontal sur un serveur d’accès au client ou de transport Edge, ou le service de transport sur un serveur de boîtes aux lettres. Pour plus d’informations sur l’architecture des rôles serveur dans Exchange 2013, voir [transport agent concepts in exchange 2013](transport-agent-concepts-in-exchange-2013.md).
    
- Les assemblys suivants pour les classes d’agent de transport :
    
  - Microsoft. Exchange. Data. dll
    
  - Microsoft. Exchange. Data. Common. dll
    
  - Microsoft. Exchange. transport. dll
    
- .NET Framework 4,5
    
Nous vous recommandons également d’installer Visual Studio 2012. Vous pouvez implémenter des agents de transport à l’aide de Visual Basic .NET ou C#.
  
## <a name="referencing-the-assemblies"></a>Référencement des assemblys
<a name="bk_ReferenceAssemblies"> </a>

Exchange 2013 fournit une bibliothèque de classes qui prennent en charge l’extension du comportement de transport Exchange. Ces classes requièrent .NET Framework 4,5. Vous pouvez implémenter des agents de transport basés sur ces classes à l’aide de Visual Studio 2012.
  
Le programme d’installation d’Exchange 2013 installe les assemblys qui sont utilisés pour le développement de l’agent de transport et les enregistre dans le global assembly cache (GAC). Pour commencer à implémenter un agent de transport, créez une référence à l’assembly Microsoft. Exchange. Data. transport dans un projet de bibliothèque de classes.
  
## <a name="implementing-a-transport-agent"></a>Implémentation d’un agent de transport
<a name="bk_implementationExample"> </a>

L’exemple suivant montre une implémentation minimale de classes qui dérivent des classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) . 
  
> [!CAUTION]
> Si plusieurs agents de transport sont installés et inscrits pour le même événement, tous les agents sont appelés, même si un agent supprime tous les destinataires d’un élément de courrier. > pour éviter les erreurs non gérées ou les comportements imprévisibles, votre agent de transport doit gérer les cas dans lesquels le nombre de destinataires d’un élément de courrier est égal à zéro. 
  
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

## <a name="installing-and-enabling-an-agent"></a>Installation et activation d’un agent
<a name="bk_InstallEnable"> </a>

Une fois que vous avez compilé votre agent sur une DLL, vous devez installer et activer l’agent sur votre serveur Exchange de développement. Dans l’environnement de commande Exchange Management Shell, utilisez l’applet de commande [install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) pour installer votre agent et la cmdlet [Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx) pour activer votre agent. Pour plus d’informations sur l’utilisation de l’environnement de commande Exchange Management Shell, consultez la rubrique [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).
  
> [!CAUTION]
> Les agents de transport ont un accès illimité aux messages électroniques qu'ils rencontrent. Exchange 2013 ne limite pas le comportement d’un agent de transport. Les agents de transport instables ou qui contiennent des failles de sécurité peuvent affecter la stabilité et la sécurité d’Exchange 2013. Par conséquent, vous devez uniquement installer des agents de transport dont vous avez entièrement confiance et qui ont été entièrement testés. 
  
Lorsque vous utilisez la cmdlet **install-TransportAgent** pour installer un agent, l’environnement de commande Exchange Management Shell conserve un verrou sur l’assembly. Pour libérer le verrou sur l’assembly, vous devez fermer l’instance de l’environnement de commande Exchange Management Shell que vous avez utilisée pour installer l’agent. Vous ne pourrez pas mettre à jour l’assembly tant que vous n’aurez pas libéré le verrou. 
  
L’exemple suivant montre comment utiliser l’environnement de commande Exchange Management Shell pour installer et activer un agent nommé MyAgent à l’aide d’une classe dérivée de [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) nommée MyAgents. MyAgentFactory. 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
Cet exemple nomme l’agent MyCustomAgent sur le serveur sur lequel l’agent est installé. L’exemple suivant montre comment activer l’agent nommé MyCustomAgent.
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
Pour gérer un agent de transport dans le service de transport frontal sur un serveur d’accès au client, ajoutez la valeur suivante à la commande : `-TransportService FrontEnd` . Par exemple, pour afficher les agents de transport dans le service de transport frontal, exécutez la commande suivante.
  
 `Get-TransportAgent -TransportService FrontEnd`
  
Pour plus d’informations sur l’installation, l’activation et la gestion de votre agent, voir [gérer les agents de transport](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Création d’un agent de transport RoutingAgent pour Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [Création d’un agent de transport SmtpReceiveAgent pour Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [Création d’un agent de transport DeliveryAgent pour Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi

- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md)   
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)
    

