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
description: L’élément Action fournit des informations qui sont utilisées pour déterminer si une autre requête de découverte automatique est requise pour retourner les informations de configuration utilisateur.
ms.openlocfilehash: 118bb59f2c929e3c74683dbf3f073da34d67a3e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756325"
---
# <a name="action-pox"></a><span data-ttu-id="55531-103">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="55531-103">Action (POX)</span></span>

<span data-ttu-id="55531-104">L’élément **Action** fournit des informations qui sont utilisées pour déterminer si une autre requête de découverte automatique est requise pour retourner les informations de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="55531-104">The **Action** element provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span> 
  
- [<span data-ttu-id="55531-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="55531-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="55531-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="55531-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="55531-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="55531-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="55531-108">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="55531-108">Action (POX)</span></span>](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="55531-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="55531-109">Attributes and elements</span></span>

<span data-ttu-id="55531-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="55531-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55531-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="55531-111">Attributes</span></span>

<span data-ttu-id="55531-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="55531-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55531-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="55531-113">Child elements</span></span>

<span data-ttu-id="55531-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="55531-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55531-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="55531-115">Parent elements</span></span>

|<span data-ttu-id="55531-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="55531-116">**Element**</span></span>|<span data-ttu-id="55531-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="55531-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55531-118">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="55531-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="55531-119">Spécifie les paramètres de compte pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="55531-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55531-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="55531-120">Text value</span></span>

<span data-ttu-id="55531-121">La valeur de texte indique si une autre requête de découverte automatique est nécessaire afin de récupérer les informations de configuration de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="55531-121">The text value represents whether another Autodiscover request is necessary to retrieve the user's configuration information.</span></span> <span data-ttu-id="55531-122">Le tableau suivant répertorie les valeurs possibles.</span><span class="sxs-lookup"><span data-stu-id="55531-122">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="55531-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="55531-123">**Value**</span></span>|<span data-ttu-id="55531-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="55531-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="55531-125">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="55531-125">redirectUrl</span></span>  <br/> |<span data-ttu-id="55531-126">Si cette valeur est spécifiée, l’élément [RedirectUrl (POX)](redirecturl-pox.md) sera spécifier l’URL de serveur d’accès au Client à utiliser dans la requête suivante de la découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="55531-126">If this value is specified, the [RedirectUrl (POX)](redirecturl-pox.md) element will specify the Client Access server URL to be used in the subsequent Autodiscover request.</span></span> <span data-ttu-id="55531-127">L’application cliente doit s’arrêter redirection après 10 redirections.</span><span class="sxs-lookup"><span data-stu-id="55531-127">The client application should stop redirecting after 10 redirects.</span></span>  <br/> |
|<span data-ttu-id="55531-128">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="55531-128">redirectAddr</span></span>  <br/> |<span data-ttu-id="55531-129">Si cette valeur est spécifiée, l’élément [RedirectAddr (POX)](redirectaddr-pox.md) devez spécifier l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante.</span><span class="sxs-lookup"><span data-stu-id="55531-129">If this value is specified, the [RedirectAddr (POX)](redirectaddr-pox.md) element will specify the e-mail address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|<span data-ttu-id="55531-130">settings</span><span class="sxs-lookup"><span data-stu-id="55531-130">settings</span></span>  <br/> |<span data-ttu-id="55531-131">Si cette valeur est spécifiée, la réponse de découverte automatique contient les paramètres qui sont utilisés pour configurer le compte.</span><span class="sxs-lookup"><span data-stu-id="55531-131">If this value is specified, the Autodiscover response contains settings that are used to configure the account.</span></span> <span data-ttu-id="55531-132">Vous trouverez la plupart des paramètres dans l’élément de [Protocole (POX)](protocol-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="55531-132">Most of the settings will be found in the [Protocol (POX)](protocol-pox.md) element.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55531-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="55531-133">See also</span></span>

- [<span data-ttu-id="55531-134">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="55531-134">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

