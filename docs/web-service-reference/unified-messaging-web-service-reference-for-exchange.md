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
ms.openlocfilehash: 12ee91c5a8b7e1ba23b937f142a9ae2835697fef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838804"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a><span data-ttu-id="ddbcd-103">Référence au service web messagerie unifiée pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ddbcd-103">Unified Messaging web service reference for Exchange</span></span>

<span data-ttu-id="ddbcd-104">Rechercher du contenu de référence pour le service web de messagerie unifiée (MU) dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-104">Find reference content for the Unified Messaging (UM) web service in Exchange.</span></span>
  
<span data-ttu-id="ddbcd-105">Le service web de messagerie unifiée (MU) fournit un point d’extensibilité qui permet aux clients lire et modifier des informations sur les propriétés de messagerie unifiée et demander qu’éléments du magasin de boîte aux lettres être analysés et dictées sur un périphérique de téléphonie.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-105">The Unified Messaging (UM) web service provides an extensibility point that enables clients to read and change information about UM properties and request that mailbox store items be parsed and dictated over a telephony device.</span></span> <span data-ttu-id="ddbcd-106">Cette section contient des informations sur les opérations et les éléments qui composent les messages XML pour le service web de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-106">This section contains information about the operations and elements that make up the XML messages for the UM web service.</span></span> <span data-ttu-id="ddbcd-107">Ce contenu s’applique à l’URL du point de terminaison de service qui est similaire à https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-107">This content applies to the service endpoint URL that is similar to https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span></span> 
  
<span data-ttu-id="ddbcd-108">Vous pouvez utiliser le service de découverte automatique pour obtenir l’URL pour le point de terminaison du service web messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-108">You can use the Autodiscover service to get the URL to the UM web service endpoint.</span></span> <span data-ttu-id="ddbcd-109">Pour plus d’informations sur la découverte automatique, voir la [découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="ddbcd-109">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="ddbcd-110">Pour les versions d’Exchange commençant par Exchange 2010, nous recommandons d’utiliser les opérations de la messagerie unifiée qui sont disponibles dans [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) au lieu du service web de messagerie unifiée, pour les raisons suivantes : > ont des fonctionnalités de la messagerie unifiée basée sur le EWS prise en charge exhaustive de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the UM web service, for the following reasons: >  The EWS-based UM features have first-class support in the EWS Managed API.</span></span> <span data-ttu-id="ddbcd-111">> Dans les versions d’Exchange commençant par Exchange 2010, les nouvelles fonctionnalités de messagerie unifiée sont ajoutées pour EWS mais pas pour le service web de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-111">>  In versions of Exchange starting with Exchange 2010, new UM features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
<span data-ttu-id="ddbcd-112">Le service web de messagerie unifiée ne dispose pas d’un schéma explicite.</span><span class="sxs-lookup"><span data-stu-id="ddbcd-112">The UM web service does not have an explicit schema.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="ddbcd-113">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="ddbcd-113">In this section</span></span>
<span data-ttu-id="ddbcd-114"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="ddbcd-114"></span></span>

- [<span data-ttu-id="ddbcd-115">Opérations du service web messagerie unifiées pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ddbcd-115">Unified Messaging web service operations for Exchange</span></span>](unified-messaging-web-service-operations-for-exchange.md)
    
- [<span data-ttu-id="ddbcd-116">Unified Messaging service XML des éléments web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ddbcd-116">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="ddbcd-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ddbcd-117">See also</span></span>

- [<span data-ttu-id="ddbcd-118">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ddbcd-118">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="ddbcd-119">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ddbcd-119">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="ddbcd-120">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ddbcd-120">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

