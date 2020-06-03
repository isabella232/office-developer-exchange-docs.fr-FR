---
title: Effectuer un suivi des demandes et des réponses pour dépanner les applications d’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 186c1d1d-b8dc-4914-b3cd-6fada7ecd877
description: Découvrez comment suivre les requêtes et les réponses EWS pour résoudre les erreurs dans votre application d’API managée EWS.
localization_priority: Priority
ms.openlocfilehash: dd225030d62a2e8211b7063ee78a59fd1a070263
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455855"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a>Effectuer un suivi des demandes et des réponses pour dépanner les applications d’API managée EWS

Découvrez comment suivre les requêtes et les réponses EWS pour résoudre les erreurs dans votre application d’API managée EWS.
  
Le débogage d’une application basée sur un service Web peut être difficile, car une partie du traitement est effectuée sur un ordinateur distant auquel vous n’avez peut-être pas accès. Étant donné que vous ne pouvez pas parcourir le code sur le serveur, il peut être utile de consulter les demandes et les réponses XML envoyées entre le client et le serveur pour déterminer quelle partie de l’application provoque une erreur. 
  
Si vous utilisez EWS, vous avez déjà accès à la demande et à la réponse XML ; vous pouvez placer un point d’arrêt dans votre code pour examiner la réponse du serveur à votre demande afin de résoudre un problème. Si vous utilisez l’API managée EWS, vous n’avez pas d’accès direct à la demande et à la réponse EWS. Toutefois, vous pouvez utiliser les méthodes de suivi sur l’objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) pour capturer la demande XML et la réponse, et vous pouvez utiliser le code XML pour déterminer la raison pour laquelle votre code ne fonctionne pas. 

Par exemple, si vous n’avez pas défini correctement une propriété, vous pouvez obtenir une réponse inattendue, et vous pouvez utiliser la sortie de suivi pour examiner la requête XML et la réponse pour identifier l’erreur. La sortie de suivi de l’API managée EWS peut également vous aider à créer manuellement la requête XML pour créer votre application EWS. Si vous utilisez EWS, vous pouvez créer une petite application à l’aide de l’API managée EWS, la suivre, puis utiliser les informations de la demande XML pour vous aider à créer votre requête EWS. 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a>Activation du suivi sur l’objet ExchangeService
<a name="bk_EnableTracing"> </a>

Pour activer le suivi, créez un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) pour votre application et définissez les propriétés de suivi comme indiqué dans l’exemple suivant. 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

Une fois que vous avez défini la propriété [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) sur **true**, toutes les demandes qui correspondent aux indicateurs de suivi seront envoyées à l’écouteur de suivi spécifié. Vous pouvez spécifier un seul indicateur de suivi, ou vous pouvez spécifier plusieurs indicateurs de suivi en les associant à un **ou**logique. Vous pouvez utiliser l' [énumération TraceFlags](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) pour spécifier des valeurs pour EWS et pour les demandes et réponses de découverte automatique. 
  
## <a name="implementing-a-tracelistener-object"></a>Implémentation d’un objet TraceListener
<a name="bk_traceListener"> </a>

Vous pouvez définir la propriété [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) sur **true** pour afficher les requêtes XML et les réponses à votre application, telles qu’une fenêtre de console. Si vous souhaitez contrôler la sortie de suivi et l’enregistrer dans un fichier, nous vous recommandons d’implémenter un objet de [classe TraceListener](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx) . L’exemple de code suivant montre un objet simple qui implémente l’interface [ITraceListener](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) et stocke les demandes et réponses suivies dans des fichiers texte ou XML. 
  
```cs
class TraceListener : ITraceListener
{
    #region ITraceListener Members
    public void Trace(string traceType, string traceMessage)
    {
      CreateXMLTextFile(traceType, traceMessage.ToString());
    }
    #endregion
    private void CreateXMLTextFile(string fileName, string traceContent)
    {
      // Create a new XML file for the trace information.
      try
      {
        // If the trace data is valid XML, create an XmlDocument object and save.
        XmlDocument xmlDoc = new XmlDocument();
        xmlDoc.Load(traceContent);
        xmlDoc.Save(fileName + ".xml");
      }
      catch
      {
        // If the trace data is not valid XML, save it as a text document.
        System.IO.File.WriteAllText(fileName + ".txt", traceContent);
      }
    }
}

```

## <a name="see-also"></a>Voir aussi

- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)    
- [Référencer l'assembly d'API managée EWS](how-to-reference-the-ews-managed-api-assembly.md)    
- [Communiquer avec EWS à l'aide de l'API managée EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

