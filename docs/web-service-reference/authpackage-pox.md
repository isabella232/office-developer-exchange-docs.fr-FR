---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: L’élément AuthPackage Spécifie le schéma d’authentification utilisé lors de l’authentification auprès du serveur Exchange qui a le rôle serveur de boîtes aux lettres.
ms.openlocfilehash: 120ec00ac82166ae2002a8fbac0edf9a1e23afc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755352"
---
# <a name="authpackage-pox"></a><span data-ttu-id="e580a-103">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="e580a-103">AuthPackage (POX)</span></span>

<span data-ttu-id="e580a-104">L’élément **AuthPackage** Spécifie le schéma d’authentification utilisé lors de l’authentification auprès du serveur Exchange qui a le rôle serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e580a-104">The **AuthPackage** element specifies the authentication scheme that is used when authenticating against the Exchange server that has the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="e580a-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="e580a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="e580a-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="e580a-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="e580a-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="e580a-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="e580a-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="e580a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="e580a-109">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="e580a-109">AuthPackage (POX)</span></span>](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="e580a-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e580a-110">Attributes and elements</span></span>

<span data-ttu-id="e580a-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e580a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e580a-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="e580a-112">Attributes</span></span>

<span data-ttu-id="e580a-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e580a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e580a-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e580a-114">Child elements</span></span>

<span data-ttu-id="e580a-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e580a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e580a-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e580a-116">Parent elements</span></span>

|<span data-ttu-id="e580a-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e580a-117">**Element**</span></span>|<span data-ttu-id="e580a-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="e580a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e580a-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="e580a-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="e580a-120">Contient les spécifications pour la connexion d’un client vers le serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="e580a-120">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e580a-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e580a-121">Text value</span></span>

<span data-ttu-id="e580a-122">La valeur texte spécifie le schéma d’authentification utilisé lors de l’authentification auprès du serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e580a-122">The text value specifies the authentication scheme that is used when authenticating against the Mailbox server.</span></span> <span data-ttu-id="e580a-123">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="e580a-123">The following are the possible values:</span></span>
  
- <span data-ttu-id="e580a-124">base</span><span class="sxs-lookup"><span data-stu-id="e580a-124">basic</span></span>
- <span data-ttu-id="e580a-125">marche</span><span class="sxs-lookup"><span data-stu-id="e580a-125">kerb</span></span>
- <span data-ttu-id="e580a-126">kerbntlm</span><span class="sxs-lookup"><span data-stu-id="e580a-126">kerbntlm</span></span>
- <span data-ttu-id="e580a-127">NTLM</span><span class="sxs-lookup"><span data-stu-id="e580a-127">ntlm</span></span>
- <span data-ttu-id="e580a-128">certificat</span><span class="sxs-lookup"><span data-stu-id="e580a-128">certificate</span></span>
- <span data-ttu-id="e580a-129">négocier</span><span class="sxs-lookup"><span data-stu-id="e580a-129">negotiate</span></span>
- <span data-ttu-id="e580a-130">nego2</span><span class="sxs-lookup"><span data-stu-id="e580a-130">nego2</span></span>
    
## <a name="remarks"></a><span data-ttu-id="e580a-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="e580a-131">Remarks</span></span>

<span data-ttu-id="e580a-132">L’élément **AuthPackage** est uniquement utilisé lorsque l’élément de [Type (POX)](type-pox.md) a pour valeur texte EXCH ou EXPR.</span><span class="sxs-lookup"><span data-stu-id="e580a-132">The **AuthPackage** element is only used when the [Type (POX)](type-pox.md) element has a text value of EXCH or EXPR.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="e580a-133">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="e580a-133">Version differences</span></span>

<span data-ttu-id="e580a-134">Office 365, Exchange Online et les versions locales d’Exchange commençant par créer 15.00.0995.014 retour une valeur de « négocier » uniquement si le serveur est configuré pour utiliser l’authentification par négociation et le client inclut un en-tête [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) qui contient « Négocier ».</span><span class="sxs-lookup"><span data-stu-id="e580a-134">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "negotiate" only if the server is configured to use Negotiate authentication and the client includes a [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "Negotiate".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e580a-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e580a-135">See also</span></span>

- [<span data-ttu-id="e580a-136">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e580a-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

