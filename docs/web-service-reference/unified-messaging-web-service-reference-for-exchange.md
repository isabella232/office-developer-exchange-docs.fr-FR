---
title: Référence au service web messagerie unifiée pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Unified
api_type:
- schema
ms.assetid: 83afea8a-c716-41df-9eb2-e1000357afb6
description: Rechercher du contenu de référence pour le service web de messagerie unifiée (MU) dans Exchange.
ms.openlocfilehash: 9e124f504ecee517edc51610696f06729904d75f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354273"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a>Référence au service web messagerie unifiée pour Exchange

Rechercher du contenu de référence pour le service web de messagerie unifiée (MU) dans Exchange.
  
Le service web de messagerie unifiée (MU) fournit un point d’extensibilité qui permet aux clients lire et modifier des informations sur les propriétés de messagerie unifiée et demander qu’éléments du magasin de boîte aux lettres être analysés et dictées sur un périphérique de téléphonie. Cette section contient des informations sur les opérations et les éléments qui composent les messages XML pour le service web de messagerie unifiée. Ce contenu s’applique à l’URL du point de terminaison de service qui est similaire à https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx. 
  
Vous pouvez utiliser le service de découverte automatique pour obtenir l’URL pour le point de terminaison du service web messagerie unifiée. Pour plus d’informations sur la découverte automatique, voir la [découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md).
  
> [!NOTE]
>  Pour les versions d’Exchange commençant par Exchange 2010, nous vous recommandons d’utiliser les opérations de la messagerie unifiée qui sont disponibles dans [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) au lieu du service web de messagerie unifiée, pour les raisons suivantes : 
> - Les fonctionnalités de la messagerie unifiée-based EWS ont la prise en charge de première classe dans l’API managée EWS. 
> - Dans les versions d’Exchange commençant par Exchange 2010, les nouvelles fonctionnalités de messagerie unifiée sont ajoutées pour EWS mais pas pour le service web de messagerie unifiée. 
  
Le service web de messagerie unifiée ne dispose pas d’un schéma explicite.
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [Opérations du service web messagerie unifiées pour Exchange](unified-messaging-web-service-operations-for-exchange.md)   
- [Unified Messaging service XML des éléments web pour Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

