---
title: Référence du service Web de découverte automatique POX pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Recherchez des informations de référence pour le service de découverte automatique POX dans Exchange.
ms.openlocfilehash: 3c0ca368f4427be7759e2db58fb418b4822dea8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465652"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Référence du service Web de découverte automatique POX pour Exchange

Recherchez des informations de référence pour le service de découverte automatique POX dans Exchange.
  
Le service de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à un serveur Exchange. Vous pouvez utiliser le service de découverte automatique « simple Old XML » (POX) pour envoyer des messages constitués uniquement de charges utiles XML, sans enveloppe SOAP englobante, afin de localiser les paramètres qu’une application cliente doit disposer afin de se connecter à Exchange.
  
> [!NOTE]
> Pour les clients qui ciblent des versions d’Exchange à partir d’Exchange Server 2010, nous vous recommandons d’utiliser le service de découverte automatique SOAP au lieu du service de découverte automatique POX. Les clients qui ciblent Exchange 2007 doivent utiliser le service de découverte automatique POX. Nous recommandons aux clients qui utilisent .NET Framework d’utiliser l’API managée EWS car elle contient un client de découverte automatique robuste et bien testé. Pour plus d’informations sur l’API managée EWS, consultez la rubrique [prise en main des applications clientes d’API managée EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Cette section fournit des informations sur les éléments XML qui sont envoyés entre le client et le serveur pendant les redirections de demande de découverte automatique de la VARIOle et les paramètres utilisateur qui sont renvoyés dans une réponse. La référence d’élément XML contient des résumés de ce que les éléments représentent et une description des hiérarchies d’éléments potentielles qui utilisent l’élément. Cette documentation couvre les instances XML qui sont envoyées entre le client et le serveur. Le service de découverte automatique POX ne dispose pas d’un schéma explicite.
  
Les Articles de cette section fournissent des exemples et des descriptions des messages qui sont utilisés pour récupérer des informations de configuration de découverte automatique à l’aide du service de découverte automatique POX. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [Demande de découverte automatique POX pour Exchange](pox-autodiscover-request-for-exchange.md)
    
- [Réponse de découverte automatique POX pour Exchange](pox-autodiscover-response-for-exchange.md)
    
- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)   
- [Référence de service Web de découverte automatique SOAP pour Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

