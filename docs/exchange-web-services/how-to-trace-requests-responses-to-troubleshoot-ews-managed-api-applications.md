---
title: Suivi des demandes et réponses pour dépanner les applications de l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 186c1d1d-b8dc-4914-b3cd-6fada7ecd877
description: Découvrez comment effectuer le suivi des demandes EWS et des réponses pour résoudre les erreurs dans votre application d’API managées.
ms.openlocfilehash: 056a1f84c4172b0404975d6fc35f9ecd7395ecdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754941"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a>Suivi des demandes et réponses pour dépanner les applications de l’API managée EWS

Découvrez comment effectuer le suivi des demandes EWS et des réponses pour résoudre les erreurs dans votre application d’API managées.
  
Débogage d’une application de service web peut être difficile, car la partie du traitement est effectuée sur un ordinateur distant qui vous n’avez pas accès à. Étant donné que vous ne pouvez pas parcourir le code sur le serveur, il peut être utile de voir les requêtes XML et les réponses qui sont envoyés entre le client et le serveur pour déterminer quelle partie de l’application qui provoque une erreur. 
  
Si vous utilisez EWS, vous avez déjà accès à la demande XML et la réponse ; Vous pouvez placer un point d’arrêt dans votre code pour passer en revue la réponse du serveur à votre requête afin de résoudre un problème. Si vous utilisez l’API managée EWS, vous n’avez pas accès direct à la demande EWS et la réponse. Toutefois, vous pouvez utiliser les méthodes de suivi sur l’objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) pour capturer la requête XML et la réponse, et vous pouvez ensuite utiliser le code XML pour déterminer pourquoi votre code ne fonctionne pas. 

Par exemple, si vous n’avez pas défini une propriété correctement, vous risquez d’obtenir une réponse inattendue et vous pouvez utiliser la sortie de trace pour examiner la requête XML et la réponse pour identifier l’erreur. La sortie de suivi de l’API managée EWS peut également vous aider à créer manuellement la demande XML pour créer votre application EWS. Si vous utilisez EWS, vous pouvez créer une petite application à l’aide des API managées remonter et puis utiliser les informations de la demande XML pour vous aider à créer votre demande EWS. 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a>Activer le suivi de l’objet ExchangeService
<a name="bk_EnableTracing"> </a>

Pour activer le suivi, créez un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) pour votre application et définir les propriétés de suivi comme indiqué dans l’exemple suivant. 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

Une fois que vous définissez la propriété [TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) sur **true**, toutes les demandes qui correspondent aux indicateurs de suivi seront envoyés à l’écouteur de trace spécifiée. Vous pouvez spécifier un indicateur de trace unique, ou vous pouvez spécifier plusieurs indicateurs de trace combinant avec un opérateur logique **OR**. Vous pouvez utiliser l' [énumération TraceFlags](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) pour spécifier des valeurs pour EWS et pour les réponses et les demandes de découverte automatique. 
  
## <a name="implementing-a-tracelistener-object"></a>Implémentation d’un objet TraceListener
<a name="bk_traceListener"> </a>

Vous pouvez définir la propriété [TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) sur **true** pour sortir les requêtes XML et les réponses à votre application, par exemple une fenêtre de console. Si vous souhaitez contrôler la sortie de trace et enregistrez-le dans un fichier, il est recommandé d’implémenter un objet de [classe TraceListener](http://msdn.microsoft.com/en-us/library/system.diagnostics.tracelistener.aspx) . L’exemple de code suivant montre un objet simple qui implémente l’interface [ITraceListener](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) et stocke les demandes de suivi et les réponses dans des fichiers texte ou XML. 
  
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
- [Référence de l’assembly de l’API managée EWS](how-to-reference-the-ews-managed-api-assembly.md)    
- [Communiquer avec EWS à l’aide de l’API managée EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

