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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455855"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a><span data-ttu-id="ab9b7-103">Effectuer un suivi des demandes et des réponses pour dépanner les applications d’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ab9b7-103">Trace requests and responses to troubleshoot EWS Managed API apps</span></span>

<span data-ttu-id="ab9b7-104">Découvrez comment suivre les requêtes et les réponses EWS pour résoudre les erreurs dans votre application d’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-104">Find out how to trace EWS requests and responses to troubleshoot errors in your EWS Managed API application.</span></span>
  
<span data-ttu-id="ab9b7-105">Le débogage d’une application basée sur un service Web peut être difficile, car une partie du traitement est effectuée sur un ordinateur distant auquel vous n’avez peut-être pas accès.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-105">Debugging a web service-based application can be difficult because part of the processing is performed on a remote computer that you might not have access to.</span></span> <span data-ttu-id="ab9b7-106">Étant donné que vous ne pouvez pas parcourir le code sur le serveur, il peut être utile de consulter les demandes et les réponses XML envoyées entre le client et le serveur pour déterminer quelle partie de l’application provoque une erreur.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-106">Because you cannot step through the code on the server, it can be helpful to see the XML requests and responses that are sent between the client and the server to determine which part of the application is causing an error.</span></span> 
  
<span data-ttu-id="ab9b7-107">Si vous utilisez EWS, vous avez déjà accès à la demande et à la réponse XML ; vous pouvez placer un point d’arrêt dans votre code pour examiner la réponse du serveur à votre demande afin de résoudre un problème.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-107">If you are using EWS, you already have access to the XML request and response; you can put a break point in your code to review the server's response to your request in order to troubleshoot an issue.</span></span> <span data-ttu-id="ab9b7-108">Si vous utilisez l’API managée EWS, vous n’avez pas d’accès direct à la demande et à la réponse EWS.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-108">If you're using the EWS Managed API, you don't have direct access to the EWS request and response.</span></span> <span data-ttu-id="ab9b7-109">Toutefois, vous pouvez utiliser les méthodes de suivi sur l’objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) pour capturer la demande XML et la réponse, et vous pouvez utiliser le code XML pour déterminer la raison pour laquelle votre code ne fonctionne pas.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-109">However, you can use tracing methods on the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object to capture the XML request and response, and you can then use the XML to determine why your code is not working.</span></span> 

<span data-ttu-id="ab9b7-110">Par exemple, si vous n’avez pas défini correctement une propriété, vous pouvez obtenir une réponse inattendue, et vous pouvez utiliser la sortie de suivi pour examiner la requête XML et la réponse pour identifier l’erreur.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-110">For example, if you did not set a property correctly, you might get an unexpected response, and you can use the trace output to look at the XML request and response to identify the error.</span></span> <span data-ttu-id="ab9b7-111">La sortie de suivi de l’API managée EWS peut également vous aider à créer manuellement la requête XML pour créer votre application EWS.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-111">The trace output from the EWS Managed API can also help you manually build the XML request to create your EWS application.</span></span> <span data-ttu-id="ab9b7-112">Si vous utilisez EWS, vous pouvez créer une petite application à l’aide de l’API managée EWS, la suivre, puis utiliser les informations de la demande XML pour vous aider à créer votre requête EWS.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-112">If you are using EWS, you can create a small application by using EWS Managed API, trace it, and then use the XML request information to help you build your EWS request.</span></span> 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a><span data-ttu-id="ab9b7-113">Activation du suivi sur l’objet ExchangeService</span><span class="sxs-lookup"><span data-stu-id="ab9b7-113">Enabling tracing on the ExchangeService object</span></span>
<span data-ttu-id="ab9b7-114"><a name="bk_EnableTracing"> </a></span><span class="sxs-lookup"><span data-stu-id="ab9b7-114"><a name="bk_EnableTracing"> </a></span></span>

<span data-ttu-id="ab9b7-115">Pour activer le suivi, créez un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) pour votre application et définissez les propriétés de suivi comme indiqué dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-115">To enable tracing, create an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for your application, and set the tracing properties as shown in the following example.</span></span> 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

<span data-ttu-id="ab9b7-116">Une fois que vous avez défini la propriété [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) sur **true**, toutes les demandes qui correspondent aux indicateurs de suivi seront envoyées à l’écouteur de suivi spécifié.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-116">After you set the [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true**, all requests that match the trace flags will be sent to the specified trace listener.</span></span> <span data-ttu-id="ab9b7-117">Vous pouvez spécifier un seul indicateur de suivi, ou vous pouvez spécifier plusieurs indicateurs de suivi en les associant à un **ou**logique.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-117">You can specify a single trace flag, or you can specify multiple trace flags by combining them with a logical **OR**.</span></span> <span data-ttu-id="ab9b7-118">Vous pouvez utiliser l' [énumération TraceFlags](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) pour spécifier des valeurs pour EWS et pour les demandes et réponses de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-118">You can use the [TraceFlags enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) to specify values for EWS and for Autodiscover requests and responses.</span></span> 
  
## <a name="implementing-a-tracelistener-object"></a><span data-ttu-id="ab9b7-119">Implémentation d’un objet TraceListener</span><span class="sxs-lookup"><span data-stu-id="ab9b7-119">Implementing a TraceListener object</span></span>
<span data-ttu-id="ab9b7-120"><a name="bk_traceListener"> </a></span><span class="sxs-lookup"><span data-stu-id="ab9b7-120"><a name="bk_traceListener"> </a></span></span>

<span data-ttu-id="ab9b7-121">Vous pouvez définir la propriété [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) sur **true** pour afficher les requêtes XML et les réponses à votre application, telles qu’une fenêtre de console.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-121">You can set the [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true** to output the XML requests and responses to your application, such as a console window.</span></span> <span data-ttu-id="ab9b7-122">Si vous souhaitez contrôler la sortie de suivi et l’enregistrer dans un fichier, nous vous recommandons d’implémenter un objet de [classe TraceListener](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ab9b7-122">If you want to control the trace output and save it to a file, we recommend that you implement a [TraceListener class](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx) object.</span></span> <span data-ttu-id="ab9b7-123">L’exemple de code suivant montre un objet simple qui implémente l’interface [ITraceListener](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) et stocke les demandes et réponses suivies dans des fichiers texte ou XML.</span><span class="sxs-lookup"><span data-stu-id="ab9b7-123">The following code example shows a simple object that implements the [ITraceListener](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) interface and stores the traced requests and responses in XML or text files.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="ab9b7-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ab9b7-124">See also</span></span>

- [<span data-ttu-id="ab9b7-125">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ab9b7-125">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
- [<span data-ttu-id="ab9b7-126">Gestion des messages d'erreur de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ab9b7-126">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)    
- [<span data-ttu-id="ab9b7-127">Référencer l'assembly d'API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ab9b7-127">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)    
- [<span data-ttu-id="ab9b7-128">Communiquer avec EWS à l'aide de l'API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ab9b7-128">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

