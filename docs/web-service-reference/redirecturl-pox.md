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
description: L’élément RedirectUrl contient l’URL de l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur Client Access installé qui doit être utilisé pour obtenir les paramètres de découverte automatique.
ms.openlocfilehash: 3b634f1a3a3d44b6aae1a826a005149200641dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829027"
---
# <a name="redirecturl-pox"></a><span data-ttu-id="08383-103">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="08383-103">RedirectUrl (POX)</span></span>

<span data-ttu-id="08383-104">L’élément **RedirectUrl** contient l’URL de l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur Client Access installé qui doit être utilisé pour obtenir les paramètres de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="08383-104">The **RedirectUrl** element contains the URL of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span> 
  
[<span data-ttu-id="08383-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="08383-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="08383-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="08383-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="08383-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="08383-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="08383-108">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="08383-108">RedirectUrl (POX)</span></span>](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="08383-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="08383-109">Attributes and elements</span></span>

<span data-ttu-id="08383-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="08383-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08383-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="08383-111">Attributes</span></span>

<span data-ttu-id="08383-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08383-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08383-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="08383-113">Child elements</span></span>

<span data-ttu-id="08383-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08383-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08383-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="08383-115">Parent elements</span></span>

|<span data-ttu-id="08383-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="08383-116">**Element**</span></span>|<span data-ttu-id="08383-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="08383-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08383-118">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="08383-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="08383-119">Spécifie les paramètres de compte pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="08383-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="08383-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="08383-120">Text value</span></span>

<span data-ttu-id="08383-121">La valeur de text représente l’URL du serveur d’accès Client qui doit être utilisé pour obtenir les paramètres de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="08383-121">The text value represents the URL of the Client Access server that should be used to obtain Autodiscover settings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="08383-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="08383-122">Remarks</span></span>

<span data-ttu-id="08383-123">L’application cliente doit s’arrêter redirection après 10 redirections.</span><span class="sxs-lookup"><span data-stu-id="08383-123">The client application should stop redirecting after 10 redirects.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="08383-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="08383-124">See also</span></span>



[<span data-ttu-id="08383-125">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="08383-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

