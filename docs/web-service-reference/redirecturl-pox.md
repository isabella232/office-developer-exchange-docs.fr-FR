---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: L’élément RedirectUrl contient l’URL de l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé et qui doit être utilisé pour obtenir les paramètres de découverte automatique.
ms.openlocfilehash: 5400b1e7a4bb7ebebc58b6a0f1fc9bf37f5a2e22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468088"
---
# <a name="redirecturl-pox"></a><span data-ttu-id="1106d-103">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1106d-103">RedirectUrl (POX)</span></span>

<span data-ttu-id="1106d-104">L’élément **redirectUrl** contient l’URL de l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé et qui doit être utilisé pour obtenir les paramètres de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="1106d-104">The **RedirectUrl** element contains the URL of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span> 
  
[<span data-ttu-id="1106d-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="1106d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="1106d-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="1106d-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="1106d-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="1106d-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="1106d-108">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1106d-108">RedirectUrl (POX)</span></span>](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1106d-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1106d-109">Attributes and elements</span></span>

<span data-ttu-id="1106d-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1106d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1106d-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="1106d-111">Attributes</span></span>

<span data-ttu-id="1106d-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1106d-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1106d-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1106d-113">Child elements</span></span>

<span data-ttu-id="1106d-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1106d-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1106d-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1106d-115">Parent elements</span></span>

|<span data-ttu-id="1106d-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1106d-116">**Element**</span></span>|<span data-ttu-id="1106d-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1106d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1106d-118">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="1106d-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="1106d-119">Spécifie les paramètres de compte de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1106d-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1106d-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="1106d-120">Text value</span></span>

<span data-ttu-id="1106d-121">La valeur de texte représente l’URL du serveur d’accès au client qui doit être utilisée pour obtenir les paramètres de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="1106d-121">The text value represents the URL of the Client Access server that should be used to obtain Autodiscover settings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1106d-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="1106d-122">Remarks</span></span>

<span data-ttu-id="1106d-123">L’application cliente doit arrêter la redirection après 10 redirections.</span><span class="sxs-lookup"><span data-stu-id="1106d-123">The client application should stop redirecting after 10 redirects.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="1106d-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1106d-124">See also</span></span>



[<span data-ttu-id="1106d-125">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="1106d-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

