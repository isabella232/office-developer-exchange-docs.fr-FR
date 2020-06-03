---
title: Package (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: L’élément package spécifie le modèle d’authentification utilisé lors de l’authentification auprès du serveur Exchange sur lequel le rôle serveur de boîtes aux lettres est installé.
ms.openlocfilehash: 5317cf49d354a558417829e1d1b5b67cd6874309
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459103"
---
# <a name="authpackage-pox"></a><span data-ttu-id="0013b-103">Package (POX)</span><span class="sxs-lookup"><span data-stu-id="0013b-103">AuthPackage (POX)</span></span>

<span data-ttu-id="0013b-104">L’élément **package** spécifie le modèle d’authentification utilisé lors de l’authentification auprès du serveur Exchange sur lequel le rôle serveur de boîtes aux lettres est installé.</span><span class="sxs-lookup"><span data-stu-id="0013b-104">The **AuthPackage** element specifies the authentication scheme that is used when authenticating against the Exchange server that has the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="0013b-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="0013b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="0013b-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="0013b-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="0013b-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="0013b-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="0013b-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="0013b-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="0013b-109">Package (POX)</span><span class="sxs-lookup"><span data-stu-id="0013b-109">AuthPackage (POX)</span></span>](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0013b-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0013b-110">Attributes and elements</span></span>

<span data-ttu-id="0013b-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0013b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0013b-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="0013b-112">Attributes</span></span>

<span data-ttu-id="0013b-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0013b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0013b-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0013b-114">Child elements</span></span>

<span data-ttu-id="0013b-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0013b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0013b-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0013b-116">Parent elements</span></span>

|<span data-ttu-id="0013b-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0013b-117">**Element**</span></span>|<span data-ttu-id="0013b-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="0013b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0013b-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="0013b-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="0013b-120">Contient les spécifications relatives à la connexion d’un client au serveur d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="0013b-120">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0013b-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0013b-121">Text value</span></span>

<span data-ttu-id="0013b-122">La valeur texte spécifie le modèle d’authentification utilisé lors de l’authentification auprès du serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0013b-122">The text value specifies the authentication scheme that is used when authenticating against the Mailbox server.</span></span> <span data-ttu-id="0013b-123">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="0013b-123">The following are the possible values:</span></span>
  
- <span data-ttu-id="0013b-124">Basic</span><span class="sxs-lookup"><span data-stu-id="0013b-124">basic</span></span>
- <span data-ttu-id="0013b-125">kerb</span><span class="sxs-lookup"><span data-stu-id="0013b-125">kerb</span></span>
- <span data-ttu-id="0013b-126">kerbntlm</span><span class="sxs-lookup"><span data-stu-id="0013b-126">kerbntlm</span></span>
- <span data-ttu-id="0013b-127">négociation</span><span class="sxs-lookup"><span data-stu-id="0013b-127">ntlm</span></span>
- <span data-ttu-id="0013b-128">certificat</span><span class="sxs-lookup"><span data-stu-id="0013b-128">certificate</span></span>
- <span data-ttu-id="0013b-129">poursuivre</span><span class="sxs-lookup"><span data-stu-id="0013b-129">negotiate</span></span>
- <span data-ttu-id="0013b-130">nego2</span><span class="sxs-lookup"><span data-stu-id="0013b-130">nego2</span></span>
    
## <a name="remarks"></a><span data-ttu-id="0013b-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="0013b-131">Remarks</span></span>

<span data-ttu-id="0013b-132">L’élément **package** est utilisé uniquement lorsque l’élément [type (POX)](type-pox.md) a une valeur de texte Exch ou Expr.</span><span class="sxs-lookup"><span data-stu-id="0013b-132">The **AuthPackage** element is only used when the [Type (POX)](type-pox.md) element has a text value of EXCH or EXPR.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="0013b-133">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="0013b-133">Version differences</span></span>

<span data-ttu-id="0013b-134">Office 365, Exchange Online et les versions locales d’Exchange commençant par Build 15.00.0995.014 renvoient la valeur « Negotiate » uniquement si le serveur est configuré pour utiliser l’authentification par négociation et si le client inclut un en-tête [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) contenant « Negotiate ».</span><span class="sxs-lookup"><span data-stu-id="0013b-134">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "negotiate" only if the server is configured to use Negotiate authentication and the client includes a [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "Negotiate".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0013b-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0013b-135">See also</span></span>

- [<span data-ttu-id="0013b-136">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0013b-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

