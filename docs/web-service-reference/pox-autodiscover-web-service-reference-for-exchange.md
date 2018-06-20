---
title: Référence de service web variole découverte automatique pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Trouvez des informations de référence pour le service de découverte automatique variole dans Exchange.
ms.openlocfilehash: a8797fe714fd23049094c3ec2475b93fec4282c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828867"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Référence de service web variole découverte automatique pour Exchange

Trouvez des informations de référence pour le service de découverte automatique variole dans Exchange.
  
Le service de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à un serveur Exchange. Vous pouvez utiliser « XML brut anciens » service de découverte automatique (POX) pour envoyer des messages qui contiennent uniquement les charges XML, sans les enveloppes SOAP englobants, afin de localiser les paramètres dont une application cliente doit se connecter à Exchange.
  
> [!NOTE]
> Pour les clients qui ciblent les versions d’Exchange commençant par Exchange Server 2010, il est recommandé que vous utilisez le service de découverte automatique SOAP au lieu du service de découverte automatique variole. Les clients qui ciblent Exchange 2007 doivent utiliser le service de découverte automatique variole. Il est recommandé que les clients qui utilisent le .NET Framework utilisent l’API managée EWS, car il contient un client de découverte automatique variole robuste et bien testé. Pour plus d’informations sur l’API managée EWS, voir [prendre en main des applications clientes API managées](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Cette section fournit des informations sur les éléments XML qui sont envoyés entre le client et le serveur au cours des redirections de demande de découverte automatique POX et les paramètres utilisateur sont retournés dans une réponse. Référence à l’élément XML contient les résumés de ce qui représentent les éléments et une description des hiérarchies d’élément potentiels qui utilisent l’élément. Cette documentation traite les instances XML qui sont envoyés entre le client et le serveur. Le service de découverte automatique variole ne dispose pas d’un schéma explicite.
  
Les articles de cette section fournissent des exemples et une description des messages qui sont utilisées pour extraire des informations de configuration de découverte automatique en utilisant le service de découverte automatique variole. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [Demande de découverte automatique variole pour Exchange](pox-autodiscover-request-for-exchange.md)
    
- [Réponse de découverte automatique variole pour Exchange](pox-autodiscover-response-for-exchange.md)
    
- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)   
- [SOAP de référence de service web de découverte automatique pour Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

