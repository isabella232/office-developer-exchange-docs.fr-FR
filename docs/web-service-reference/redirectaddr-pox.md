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
description: L’élément RedirectAddr spécifie l’adresse de messagerie qui doit être utilisée pour une demande de découverte automatique ultérieure.
ms.openlocfilehash: 6bff28001851f421b4c7429770185401f2f0a743
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529874"
---
# <a name="redirectaddr-pox"></a><span data-ttu-id="ca4be-103">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="ca4be-103">RedirectAddr (POX)</span></span>

<span data-ttu-id="ca4be-104">L’élément **RedirectAddr** spécifie l’adresse de messagerie qui doit être utilisée pour une demande de découverte automatique ultérieure.</span><span class="sxs-lookup"><span data-stu-id="ca4be-104">The **RedirectAddr** element specifies the e-mail address that should be used for a subsequent Autodiscover request.</span></span> 
  
[<span data-ttu-id="ca4be-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="ca4be-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="ca4be-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="ca4be-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="ca4be-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="ca4be-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="ca4be-108">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="ca4be-108">RedirectAddr (POX)</span></span>](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ca4be-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ca4be-109">Attributes and elements</span></span>

<span data-ttu-id="ca4be-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ca4be-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca4be-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="ca4be-111">Attributes</span></span>

<span data-ttu-id="ca4be-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ca4be-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca4be-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ca4be-113">Child elements</span></span>

<span data-ttu-id="ca4be-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ca4be-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ca4be-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ca4be-115">Parent elements</span></span>

|<span data-ttu-id="ca4be-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ca4be-116">**Element**</span></span>|<span data-ttu-id="ca4be-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ca4be-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca4be-118">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="ca4be-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="ca4be-119">Spécifie les paramètres de compte de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ca4be-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ca4be-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ca4be-120">Text value</span></span>

<span data-ttu-id="ca4be-121">La valeur de texte représente l’adresse de messagerie qui doit être utilisée pour une demande de découverte automatique ultérieure.</span><span class="sxs-lookup"><span data-stu-id="ca4be-121">The text value represents the e-mail address that should be used for a subsequent Autodiscover request.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ca4be-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="ca4be-122">Remarks</span></span>

<span data-ttu-id="ca4be-123">Si cet élément est présent dans la réponse de découverte automatique, effectuez une autre demande à l’aide de la valeur de texte de l’élément **RedirectAddr** .</span><span class="sxs-lookup"><span data-stu-id="ca4be-123">If this element is present in the Autodiscover response, make another request by using the text value of the **RedirectAddr** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ca4be-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ca4be-124">See also</span></span>



[<span data-ttu-id="ca4be-125">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ca4be-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

