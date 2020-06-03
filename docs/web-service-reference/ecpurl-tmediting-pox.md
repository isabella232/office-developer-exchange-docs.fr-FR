---
title: EcpUrl-tmEditing (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: L’élément EcpUrl-tmEditing spécifie une URL partielle qui peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante.
ms.openlocfilehash: 5d6c6b8e8f73d113cfde3570065435927ffbae05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463537"
---
# <a name="ecpurl-tmediting-pox"></a><span data-ttu-id="74d65-103">EcpUrl-tmEditing (POX)</span><span class="sxs-lookup"><span data-stu-id="74d65-103">EcpUrl-tmEditing (POX)</span></span>

<span data-ttu-id="74d65-104">L’élément **EcpUrl-tmEditing** spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante.</span><span class="sxs-lookup"><span data-stu-id="74d65-104">The **EcpUrl-tmEditing** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span> 
  
[<span data-ttu-id="74d65-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="74d65-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="74d65-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="74d65-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="74d65-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="74d65-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="74d65-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="74d65-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="74d65-109">EcpUrl-tmEditing (POX)</span><span class="sxs-lookup"><span data-stu-id="74d65-109">EcpUrl-tmEditing (POX)</span></span>](ecpurl-tmediting-pox.md)
  
```XML
<EcpUrl-tmEditing/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="74d65-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="74d65-110">Attributes and elements</span></span>

<span data-ttu-id="74d65-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="74d65-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74d65-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="74d65-112">Attributes</span></span>

<span data-ttu-id="74d65-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="74d65-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74d65-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="74d65-114">Child elements</span></span>

<span data-ttu-id="74d65-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="74d65-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="74d65-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="74d65-116">Parent elements</span></span>

|<span data-ttu-id="74d65-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="74d65-117">**Element**</span></span>|<span data-ttu-id="74d65-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="74d65-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74d65-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="74d65-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="74d65-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="74d65-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74d65-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="74d65-121">Text value</span></span>

<span data-ttu-id="74d65-122">La valeur de texte représente une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante.</span><span class="sxs-lookup"><span data-stu-id="74d65-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span> <span data-ttu-id="74d65-123">La valeur de l’élément **EcpUrl-tmEditing** contient les paramètres contenus dans les caractères « < » et « > » qui sont remplacés par le client, comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="74d65-123">The value of the **EcpUrl-tmEditing** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="74d65-124">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="74d65-124">**Parameter**</span></span>|<span data-ttu-id="74d65-125">**Remplacer par**</span><span class="sxs-lookup"><span data-stu-id="74d65-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="74d65-126">_Id_</span><span class="sxs-lookup"><span data-stu-id="74d65-126">_Id_</span></span> <br/> |<span data-ttu-id="74d65-127">Adresse de messagerie SMTP ou nom unique X500 de la boîte aux lettres de site.</span><span class="sxs-lookup"><span data-stu-id="74d65-127">The SMTP email address or the X500 distinguished name of the site mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="74d65-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="74d65-128">Remarks</span></span>

<span data-ttu-id="74d65-129">L’élément **EcpUrl-tmEditing** est un élément enfant facultatif de l’élément **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="74d65-129">The **EcpUrl-tmEditing** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="74d65-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="74d65-130">See also</span></span>



[<span data-ttu-id="74d65-131">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="74d65-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

