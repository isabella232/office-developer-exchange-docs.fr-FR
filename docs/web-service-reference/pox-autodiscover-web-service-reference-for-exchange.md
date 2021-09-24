---
title: Référence du service web de découverte automatique POX pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Recherchez des informations de référence pour le service de découverte automatique POX dans Exchange.
ms.openlocfilehash: b28ea64a82960a84dee06c5055ee915614f4fde7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516418"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Référence du service web de découverte automatique POX pour Exchange

Recherchez des informations de référence pour le service de découverte automatique POX dans Exchange.
  
Le service de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à Exchange serveur. Vous pouvez utiliser le service de découverte automatique « plain old XML » (POX) pour envoyer des messages qui se composent uniquement de charges utiles XML, sans enveloppe SOAP incluse, afin de localiser les paramètres dont une application cliente doit avoir pour se connecter à Exchange.
  
> [!NOTE]
> Pour les clients qui ciblent des versions de Exchange à partir de Exchange Server 2010, nous vous recommandons d’utiliser le service de découverte automatique SOAP au lieu du service de découverte automatique POX. Les clients qui ciblent Exchange 2007 doivent utiliser le service de découverte automatique POX. Nous recommandons aux clients qui utilisent le .NET Framework l’API gérée EWS, car elle contient un client de découverte automatique POX robuste et bien testé. Pour plus d’informations sur l’API gérée EWS, voir Get [started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Cette section fournit des informations sur les éléments XML qui sont envoyés entre le client et le serveur pendant les redirections de demande de découverte automatique POX et les paramètres utilisateur renvoyés dans une réponse. La référence d’élément XML contient des résumés de ce que représentent les éléments et une description des hiérarchies d’éléments potentielles qui utilisent l’élément. Cette documentation couvre les instances XML qui sont envoyées entre le client et le serveur. Le service de découverte automatique POX ne comprend pas de schéma explicite.
  
Les articles de cette section fournissent des exemples et des descriptions des messages utilisés pour récupérer des informations de configuration de découverte automatique à l’aide du service de découverte automatique POX. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [Demande de découverte automatique POX pour Exchange](pox-autodiscover-request-for-exchange.md)
    
- [Réponse de découverte automatique POX pour Exchange](pox-autodiscover-response-for-exchange.md)
    
- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)   
- [Référence du service web de découverte automatique SOAP pour Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

