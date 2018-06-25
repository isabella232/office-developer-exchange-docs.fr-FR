---
title: Référence de service web de découverte automatique pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a01124a8-a8cf-4b80-8625-d7ee05690bca
description: Rechercher du contenu de référence pour le service web de découverte automatique dans Exchange.
ms.openlocfilehash: 48ca4a93c2120079cb675eabbc460bf0e75570b2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755358"
---
# <a name="autodiscover-web-service-reference-for-exchange"></a>Référence de service web de découverte automatique pour Exchange

Rechercher du contenu de référence pour le service web de découverte automatique dans Exchange.
  
Le service web de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à un serveur Exchange. Vous pouvez utiliser une des options suivantes pour se connecter au service de découverte automatique :
  
- Service de découverte automatique SOAP — pour les clients qui se connectent à des versions d’Exchange commençant par Exchange 2010, notamment Exchange Online.
    
- « XML brut ancienne » service de découverte automatique (POX) — pour les clients qui se connectent à des versions d’Exchange commençant par Exchange 2007, notamment Exchange Online. 
    
À la fois le protocole SOAP et le service de découverte automatique variole peuvent fournir les informations de configuration que votre client utilisera pour créer une connexion à un serveur Exchange.
  
> [!NOTE]
> Pour les versions d’Exchange commençant par Exchange 2010, il est recommandé que vous utilisez le service de découverte automatique SOAP au lieu du service de découverte automatique variole. Le service de découverte automatique SOAP fournit des requêtes de paramètre Autodiscover groupées et un contrôle plus précis sur les paramètres sont retournés dans la réponse. 
  
Cette section contient des informations de référence pour le service de découverte automatique SOAP et le service de découverte automatique variole.
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [SOAP de référence de service web de découverte automatique pour Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
    
- [Référence de service web variole découverte automatique pour Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Référence des services web pour Exchange](web-services-reference-for-exchange.md)
- [Service de découverte automatique (SOAP)](http://msdn.microsoft.com/library/e24d1a1f-0d20-4bd9-ae4c-9112ecacea78%28Office.15%29.aspx)
- [Service de découverte automatique (POX)](http://msdn.microsoft.com/library/13c54de3-a91c-4424-8732-99dd8f2162ec%28Office.15%29.aspx)
    

