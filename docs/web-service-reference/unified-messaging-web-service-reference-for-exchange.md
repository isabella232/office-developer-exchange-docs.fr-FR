---
title: Référence du service Web de messagerie unifiée pour Exchange
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
description: Recherchez du contenu de référence pour le service Web de messagerie unifiée dans Exchange.
ms.openlocfilehash: e4bb63f34650dae8fc28016196c97a6b79e69df0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467374"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a><span data-ttu-id="e0cdd-103">Référence du service Web de messagerie unifiée pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e0cdd-103">Unified Messaging web service reference for Exchange</span></span>

<span data-ttu-id="e0cdd-104">Recherchez du contenu de référence pour le service Web de messagerie unifiée dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0cdd-104">Find reference content for the Unified Messaging (UM) web service in Exchange.</span></span>
  
<span data-ttu-id="e0cdd-105">Le service Web de messagerie unifiée fournit un point d’extensibilité qui permet aux clients de lire et de modifier des informations sur les propriétés de messagerie unifiée et de demander que les éléments de la Banque de boîtes aux lettres soient analysés et dictés sur un appareil de téléphonie.</span><span class="sxs-lookup"><span data-stu-id="e0cdd-105">The Unified Messaging (UM) web service provides an extensibility point that enables clients to read and change information about UM properties and request that mailbox store items be parsed and dictated over a telephony device.</span></span> <span data-ttu-id="e0cdd-106">Cette section contient des informations sur les opérations et les éléments qui composent les messages XML pour le service Web de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="e0cdd-106">This section contains information about the operations and elements that make up the XML messages for the UM web service.</span></span> <span data-ttu-id="e0cdd-107">Ce contenu s’applique à l’URL de point de terminaison de service qui est similaire à https:// \<yourclientaccessserver\> . com/EWS/UM2007Legacy. asmx.</span><span class="sxs-lookup"><span data-stu-id="e0cdd-107">This content applies to the service endpoint URL that is similar to https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span></span> 
  
<span data-ttu-id="e0cdd-108">Vous pouvez utiliser le service de découverte automatique pour obtenir l’URL du point de terminaison du service Web de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="e0cdd-108">You can use the Autodiscover service to get the URL to the UM web service endpoint.</span></span> <span data-ttu-id="e0cdd-109">Pour plus d’informations sur la découverte automatique, consultez la rubrique [découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="e0cdd-109">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="e0cdd-110">Pour les versions d’Exchange commençant par Exchange 2010, nous vous recommandons d’utiliser les opérations de messagerie unifiée disponibles dans les [services Web Exchange (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) au lieu du service Web de messagerie unifiée, pour les raisons suivantes :</span><span class="sxs-lookup"><span data-stu-id="e0cdd-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the UM web service, for the following reasons:</span></span> 
> - <span data-ttu-id="e0cdd-111">Les fonctionnalités de messagerie unifiée EWS ont une prise en charge de première classe dans l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="e0cdd-111">The EWS-based UM features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="e0cdd-112">Dans les versions d’Exchange à partir d’Exchange 2010, les nouvelles fonctionnalités de messagerie UNIFIÉe sont ajoutées à EWS, mais pas au service Web de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="e0cdd-112">In versions of Exchange starting with Exchange 2010, new UM features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
<span data-ttu-id="e0cdd-113">Le service Web de messagerie unifiée n’a pas de schéma explicite.</span><span class="sxs-lookup"><span data-stu-id="e0cdd-113">The UM web service does not have an explicit schema.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="e0cdd-114">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="e0cdd-114">In this section</span></span>
<span data-ttu-id="e0cdd-115"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="e0cdd-115"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="e0cdd-116">Opérations de service Web de messagerie unifiée pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e0cdd-116">Unified Messaging web service operations for Exchange</span></span>](unified-messaging-web-service-operations-for-exchange.md)   
- [<span data-ttu-id="e0cdd-117">Éléments XML de service Web de messagerie unifiée pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e0cdd-117">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="e0cdd-118">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e0cdd-118">See also</span></span>

- [<span data-ttu-id="e0cdd-119">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e0cdd-119">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="e0cdd-120">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e0cdd-120">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="e0cdd-121">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e0cdd-121">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

