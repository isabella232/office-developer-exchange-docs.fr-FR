---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: L’élément EcpUrl-tmHiding spécifie une URL partielle peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres du site.
ms.openlocfilehash: 461e9780dbd657ba0ba8b9ce9ea4fe902cba9698
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756074"
---
# <a name="ecpurl-tmhiding-pox"></a><span data-ttu-id="9af35-103">EcpUrl-tmHiding (POX)</span><span class="sxs-lookup"><span data-stu-id="9af35-103">EcpUrl-tmHiding (POX)</span></span>

<span data-ttu-id="9af35-104">L’élément **EcpUrl-tmHiding** spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres du site.</span><span class="sxs-lookup"><span data-stu-id="9af35-104">The **EcpUrl-tmHiding** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span> 
  
[<span data-ttu-id="9af35-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="9af35-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="9af35-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="9af35-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="9af35-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="9af35-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="9af35-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="9af35-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="9af35-109">EcpUrl-tmHiding (POX)</span><span class="sxs-lookup"><span data-stu-id="9af35-109">EcpUrl-tmHiding (POX)</span></span>](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9af35-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9af35-110">Attributes and elements</span></span>

<span data-ttu-id="9af35-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9af35-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9af35-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="9af35-112">Attributes</span></span>

<span data-ttu-id="9af35-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9af35-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9af35-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9af35-114">Child elements</span></span>

<span data-ttu-id="9af35-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9af35-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9af35-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9af35-116">Parent elements</span></span>

|<span data-ttu-id="9af35-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9af35-117">**Element**</span></span>|<span data-ttu-id="9af35-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="9af35-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9af35-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="9af35-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="9af35-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="9af35-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9af35-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9af35-121">Text value</span></span>

<span data-ttu-id="9af35-122">La valeur de texte représente une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres du site.</span><span class="sxs-lookup"><span data-stu-id="9af35-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span> <span data-ttu-id="9af35-123">La valeur de l’élément **EcpUrl-tmHiding** contient les paramètres contenus dans « < » et « > » caractères sont remplacés par le client, comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="9af35-123">The value of the **EcpUrl-tmHiding** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="9af35-124">**Paramètre**</span><span class="sxs-lookup"><span data-stu-id="9af35-124">**Parameter**</span></span>|<span data-ttu-id="9af35-125">**Remplacer par**</span><span class="sxs-lookup"><span data-stu-id="9af35-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="9af35-126">
  _Id_</span><span class="sxs-lookup"><span data-stu-id="9af35-126">_Id_</span></span> <br/> |<span data-ttu-id="9af35-127">L’adresse de messagerie SMTP ou la X500 le nom de la boîte aux lettres de site unique.</span><span class="sxs-lookup"><span data-stu-id="9af35-127">The SMTP email address or the X500 distinguished name of the site mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9af35-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="9af35-128">Remarks</span></span>

<span data-ttu-id="9af35-129">L’élément **EcpUrl-tmHiding** est un élément enfant facultatif de l’élément de **protocole** .</span><span class="sxs-lookup"><span data-stu-id="9af35-129">The **EcpUrl-tmHiding** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="9af35-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9af35-130">See also</span></span>



[<span data-ttu-id="9af35-131">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="9af35-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

