---
title: Action (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: L’élément action fournit des informations qui permettent de déterminer si une autre demande de découverte automatique est nécessaire pour renvoyer les informations de configuration de l’utilisateur.
ms.openlocfilehash: f6d542b908948d09020b850b60ca1bdb025dd342
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529692"
---
# <a name="action-pox"></a><span data-ttu-id="46893-103">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="46893-103">Action (POX)</span></span>

<span data-ttu-id="46893-104">L’élément **action** fournit des informations qui permettent de déterminer si une autre demande de découverte automatique est nécessaire pour renvoyer les informations de configuration de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="46893-104">The **Action** element provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span> 
  
- [<span data-ttu-id="46893-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="46893-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="46893-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="46893-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="46893-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="46893-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="46893-108">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="46893-108">Action (POX)</span></span>](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="46893-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="46893-109">Attributes and elements</span></span>

<span data-ttu-id="46893-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="46893-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46893-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="46893-111">Attributes</span></span>

<span data-ttu-id="46893-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="46893-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46893-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="46893-113">Child elements</span></span>

<span data-ttu-id="46893-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="46893-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="46893-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="46893-115">Parent elements</span></span>

|<span data-ttu-id="46893-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="46893-116">**Element**</span></span>|<span data-ttu-id="46893-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="46893-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46893-118">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="46893-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="46893-119">Spécifie les paramètres de compte de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="46893-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="46893-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="46893-120">Text value</span></span>

<span data-ttu-id="46893-121">La valeur de texte indique si une autre demande de découverte automatique est nécessaire pour récupérer les informations de configuration de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="46893-121">The text value represents whether another Autodiscover request is necessary to retrieve the user's configuration information.</span></span> <span data-ttu-id="46893-122">Le tableau suivant répertorie les valeurs possibles.</span><span class="sxs-lookup"><span data-stu-id="46893-122">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="46893-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="46893-123">**Value**</span></span>|<span data-ttu-id="46893-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="46893-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="46893-125">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="46893-125">redirectUrl</span></span>  <br/> |<span data-ttu-id="46893-126">Si cette valeur est spécifiée, l’élément [redirectUrl (POX)](redirecturl-pox.md) spécifie l’URL du serveur d’accès au client à utiliser dans la demande de découverte automatique suivante.</span><span class="sxs-lookup"><span data-stu-id="46893-126">If this value is specified, the [RedirectUrl (POX)](redirecturl-pox.md) element will specify the Client Access server URL to be used in the subsequent Autodiscover request.</span></span> <span data-ttu-id="46893-127">L’application cliente doit arrêter la redirection après 10 redirections.</span><span class="sxs-lookup"><span data-stu-id="46893-127">The client application should stop redirecting after 10 redirects.</span></span>  <br/> |
|<span data-ttu-id="46893-128">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="46893-128">redirectAddr</span></span>  <br/> |<span data-ttu-id="46893-129">Si cette valeur est spécifiée, l’élément [RedirectAddr (POX)](redirectaddr-pox.md) indique l’adresse de messagerie qui doit être utilisée pour une demande de découverte automatique ultérieure.</span><span class="sxs-lookup"><span data-stu-id="46893-129">If this value is specified, the [RedirectAddr (POX)](redirectaddr-pox.md) element will specify the e-mail address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|<span data-ttu-id="46893-130">paramètres</span><span class="sxs-lookup"><span data-stu-id="46893-130">settings</span></span>  <br/> |<span data-ttu-id="46893-131">Si cette valeur est spécifiée, la réponse de découverte automatique contient les paramètres qui sont utilisés pour configurer le compte.</span><span class="sxs-lookup"><span data-stu-id="46893-131">If this value is specified, the Autodiscover response contains settings that are used to configure the account.</span></span> <span data-ttu-id="46893-132">La plupart des paramètres seront disponibles dans l’élément [Protocol (POX)](protocol-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="46893-132">Most of the settings will be found in the [Protocol (POX)](protocol-pox.md) element.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46893-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="46893-133">See also</span></span>

- [<span data-ttu-id="46893-134">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="46893-134">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

