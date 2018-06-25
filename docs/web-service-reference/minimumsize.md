---
title: MinimumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: L’élément MinimumSize représente la taille minimale doit correspondre à un message afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 4f80bac3b9226019ec3d726cd2d6430e02cac423
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828480"
---
# <a name="minimumsize"></a><span data-ttu-id="69bef-103">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="69bef-103">MinimumSize</span></span>

<span data-ttu-id="69bef-104">L’élément **MinimumSize** représente la taille minimale doit correspondre à un message afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="69bef-104">The **MinimumSize** element represents the minimum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<MinimumSize/>
```

 <span data-ttu-id="69bef-105">**int**</span><span class="sxs-lookup"><span data-stu-id="69bef-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69bef-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="69bef-106">Attributes and elements</span></span>

<span data-ttu-id="69bef-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="69bef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69bef-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="69bef-108">Attributes</span></span>

<span data-ttu-id="69bef-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="69bef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69bef-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="69bef-110">Child elements</span></span>

<span data-ttu-id="69bef-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="69bef-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="69bef-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="69bef-112">Parent elements</span></span>

|<span data-ttu-id="69bef-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="69bef-113">**Element**</span></span>|<span data-ttu-id="69bef-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="69bef-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69bef-115">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="69bef-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="69bef-116">Spécifie les tailles minimales et maximales des messages entrants doivent être dans l’ordre de l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="69bef-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="69bef-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="69bef-117">Text value</span></span>

<span data-ttu-id="69bef-118">La valeur de texte est un entier qui identifie la taille minimale du message en octets.</span><span class="sxs-lookup"><span data-stu-id="69bef-118">The text value is an integer that identifies the minimum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="69bef-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="69bef-119">Remarks</span></span>

<span data-ttu-id="69bef-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="69bef-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69bef-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="69bef-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69bef-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="69bef-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="69bef-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="69bef-123">Schema Name</span></span>  <br/> |<span data-ttu-id="69bef-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="69bef-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="69bef-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="69bef-125">Validation File</span></span>  <br/> |<span data-ttu-id="69bef-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="69bef-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="69bef-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="69bef-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="69bef-128">True</span><span class="sxs-lookup"><span data-stu-id="69bef-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69bef-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="69bef-129">See also</span></span>



[<span data-ttu-id="69bef-130">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="69bef-130">MaximumSize</span></span>](maximumsize.md)


- [<span data-ttu-id="69bef-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="69bef-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

