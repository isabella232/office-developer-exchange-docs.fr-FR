---
title: RedirectAddr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4
description: L’élément RedirectAddr Spécifie l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante.
ms.openlocfilehash: fe15054b9962fc2decf52ac3c42536e36358948a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829020"
---
# <a name="redirectaddr-pox"></a><span data-ttu-id="08c7b-103">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="08c7b-103">RedirectAddr (POX)</span></span>

<span data-ttu-id="08c7b-104">L’élément **RedirectAddr** Spécifie l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante.</span><span class="sxs-lookup"><span data-stu-id="08c7b-104">The **RedirectAddr** element specifies the e-mail address that should be used for a subsequent Autodiscover request.</span></span> 
  
[<span data-ttu-id="08c7b-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="08c7b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="08c7b-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="08c7b-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="08c7b-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="08c7b-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="08c7b-108">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="08c7b-108">RedirectAddr (POX)</span></span>](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="08c7b-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="08c7b-109">Attributes and elements</span></span>

<span data-ttu-id="08c7b-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="08c7b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08c7b-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="08c7b-111">Attributes</span></span>

<span data-ttu-id="08c7b-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08c7b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08c7b-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="08c7b-113">Child elements</span></span>

<span data-ttu-id="08c7b-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08c7b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08c7b-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="08c7b-115">Parent elements</span></span>

|<span data-ttu-id="08c7b-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="08c7b-116">**Element**</span></span>|<span data-ttu-id="08c7b-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="08c7b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08c7b-118">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="08c7b-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="08c7b-119">Spécifie les paramètres de compte pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="08c7b-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="08c7b-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="08c7b-120">Text value</span></span>

<span data-ttu-id="08c7b-121">La valeur de text représente l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante.</span><span class="sxs-lookup"><span data-stu-id="08c7b-121">The text value represents the e-mail address that should be used for a subsequent Autodiscover request.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="08c7b-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="08c7b-122">Remarks</span></span>

<span data-ttu-id="08c7b-123">Si cet élément est présent dans la réponse de découverte automatique, effectuer une autre demande à l’aide de la valeur de texte de l’élément **RedirectAddr** .</span><span class="sxs-lookup"><span data-stu-id="08c7b-123">If this element is present in the Autodiscover response, make another request by using the text value of the **RedirectAddr** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="08c7b-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="08c7b-124">See also</span></span>



[<span data-ttu-id="08c7b-125">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="08c7b-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

