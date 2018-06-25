---
title: Création d’agents de transport pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Trouvez des informations sur la création des agents de transport personnalisés pour Exchange 2013 et la configuration système requise pour la création d’un agent personnalisé.
ms.openlocfilehash: 6146e37c44441bed1d30d08f71ede255dba26440
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755119"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Création d’agents de transport pour Exchange 2013

Trouvez des informations sur la création des agents de transport personnalisés pour Exchange 2013 et la configuration système requise pour la création d’un agent personnalisé.
  
**S’applique à :** Exchange Server 2013
  
Exchange Server 2013 inclut plusieurs agents de transport que vous pouvez utiliser pour traiter les messages. En utilisant les assemblys qui sont fournis avec Exchange, vous pouvez créer vos propres agents personnalisés pour exécuter des tâches spécifiques en fonction des besoins de votre organisation. Par exemple, vous pouvez utiliser un agent de transport SmtpReceiveAgent pour intercepter les messages reçus par le biais du protocole SMTP et le processus le message pour convertir le format du corps pour contenir le texte préformaté. Vous pouvez utiliser un agent de transport RoutingAgent pour consigner les messages qui transitent par le serveur sur l’itinéraire vers un autre serveur. Vous pouvez également créer plus complexe fonctionnalités qui facilitent l’utilisent de plusieurs types d’agents. Par exemple, pour créer un agent antiviru, vous pouvez implémenter un SmtpReceiveAgent et un agent RoutingAgent. Si vous avez un composant sur votre réseau ne prend pas en charge le protocole SMTP, vous pouvez utiliser un agent de transport DeliveryAgent pour traiter la communication entre votre serveur Exchange et votre composant externe. 
  
Cet article fournit des informations sur les conditions requises pour les tâches impliquées dans la création de votre propre agent de transport. Pour plus d’informations sur la création des agents de transport spécifique, voir [créer un agent de transport RoutingAgent pour Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [créer un agent de transport SmtpReceiveAgent pour Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)et [créer un agent de transport DeliveryAgent pour Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>Conditions requises pour créer un agent de transport
<a name="bk_prerequisites"> </a>

Les conditions préalables que vous avez besoin pour mettre en œuvre un agent de transport sont les suivantes :
  
- Un ordinateur qui exécute Exchange 2013 qui exécute le service de Transport frontal sur un serveur d’accès au Client ou de Transport Edge ou le service de Transport sur un serveur de boîtes aux lettres. Pour plus d’informations sur l’architecture du rôle de serveur dans Exchange 2013, voir [Concepts relatifs aux agents de Transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md).
    
- Les assemblys suivants pour les classes de l’agent de transport :
    
  - Microsoft.Exchange.Data.dll
    
  - Microsoft.Exchange.Data.Common.dll
    
  - Microsoft.Exchange.Transport.dll
    
- Le .NET Framework 4.5
    
Nous vous recommandons également d’installer Visual Studio 2012. Vous pouvez implémenter des agents de transport à l’aide de Visual Basic .NET ou c#.
  
## <a name="referencing-the-assemblies"></a>Référencement des assemblys
<a name="bk_ReferenceAssemblies"> </a>

Exchange 2013 fournit une bibliothèque de classes qui prennent en charge l’extension de comportement de transport Exchange. Ces classes nécessitent le .NET Framework 4.5. Vous pouvez implémenter des agents de transport en fonction de ces classes à l’aide de Visual Studio 2012.
  
Le programme d’installation Exchange 2013 installe les assemblys qui sont utilisés pour le développement de l’agent de transport et les enregistre dans le global assembly cache (GAC). Pour commencer à créer un agent de transport, créez une référence à l’assembly Microsoft.Exchange.Data.Transport dans un projet de bibliothèque de classes.
  
## <a name="implementing-a-transport-agent"></a>L’implémentation d’un agent de transport
<a name="bk_implementationExample"> </a>

L’exemple suivant montre une implémentation minimale de classes dérivées des classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) . 
  
> [!CAUTION]
> Si plusieurs agents de transport sont installés et inscrits pour l’événement de même, tous les agents seront appelés, même si un agent supprime tous les destinataires d’un élément de messagerie. > Pour éviter les erreurs non traitées ou un comportement imprévisible, l’agent de transport doit gérer les cas dans lesquels le nombre de destinataires dans un élément de courrier est égal à zéro. 
  
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

Après avoir compilé votre agent d’une DLL, vous devez installer et activer l’agent sur votre serveur Exchange de développement. Dans Exchange Management Shell, utilisez l’applet de commande [Install-TransportAgent](http://technet.microsoft.com/en-us/library/aa997998.aspx) pour installer l’agent et l’applet de commande [Enable-TransportAgent](http://technet.microsoft.com/en-us/library/bb124921.aspx) pour activer l’agent. Pour plus d’informations sur l’utilisation d’Exchange Management Shell, voir [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).
  
> [!CAUTION]
> Agents de transport ont un accès complet à tous les messages électroniques qu’ils rencontrent. Exchange 2013 ne restreint pas le comportement d’un agent de transport. Agents de transport qui sont instables ou qui contiennent les failles de sécurité peuvent affecter la stabilité et la sécurité d’Exchange 2013. Par conséquent, vous devez installer uniquement les agents de transport entièrement fiable et qui ont été testés. 
  
Lorsque vous utilisez l’applet de commande **Install-TransportAgent** pour installer un agent, Exchange Management Shell conserve un verrou sur l’assembly. Pour libérer le verrou sur l’assembly, vous devez fermer l’instance d’Exchange Management Shell que vous avez utilisé pour installer l’agent. Vous ne pourrez pas mettre à jour l’assembly jusqu'à ce que vous relâchiez le verrou. 
  
L’exemple suivant montre comment utiliser l’environnement Exchange Management Shell pour installer et activer un agent nommé MyAgent à l’aide d’une classe dérivée de [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) nommé MyAgents.MyAgentFactory. 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
Cet exemple montre comment les noms l’agent MyCustomAgent sur le serveur sur lequel l’agent est installé. L’exemple suivant montre comment activer l’agent nommé MyCustomAgent.
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
Pour gérer un agent de transport dans le service de Transport frontal sur un serveur d’accès au Client, ajoutez la valeur suivante à la commande : `-TransportService FrontEnd`. Par exemple, pour afficher les agents de transport dans le service de Transport frontal, exécutez la commande suivante.
  
 `Get-TransportAgent -TransportService FrontEnd`
  
Pour plus d’informations sur l’installation, l’activation et la gestion de l’agent, voir [Gérer les Agents de Transport](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx).
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Créer un agent de transport RoutingAgent pour Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [Créer un agent de transport SmtpReceiveAgent pour Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [Créer un agent de transport DeliveryAgent pour Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi

- [Concepts de l’agent d’Exchange 2013 de transport](transport-agent-concepts-in-exchange-2013.md)   
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)
    

