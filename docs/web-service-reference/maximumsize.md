---
title: /M
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fb7c3ab3-ef97-44c7-83e0-93cfe8c48e84
description: L’élément MaximumSize représente la taille maximale qu’un message doit être pour que la condition ou l’exception s’applique.
ms.openlocfilehash: 250e0c6aed37b934f5cf6eaed9d93b9f56159d93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461750"
---
# <a name="maximumsize"></a><span data-ttu-id="02b39-103">/M</span><span class="sxs-lookup"><span data-stu-id="02b39-103">MaximumSize</span></span>

<span data-ttu-id="02b39-104">L’élément **MaximumSize** représente la taille maximale qu’un message doit être pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="02b39-104">The **MaximumSize** element represents the maximum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<Maximum/>
```

 <span data-ttu-id="02b39-105">**int**</span><span class="sxs-lookup"><span data-stu-id="02b39-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02b39-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="02b39-106">Attributes and elements</span></span>

<span data-ttu-id="02b39-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="02b39-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02b39-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="02b39-108">Attributes</span></span>

<span data-ttu-id="02b39-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="02b39-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02b39-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="02b39-110">Child elements</span></span>

<span data-ttu-id="02b39-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="02b39-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="02b39-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="02b39-112">Parent elements</span></span>

|<span data-ttu-id="02b39-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="02b39-113">**Element**</span></span>|<span data-ttu-id="02b39-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="02b39-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02b39-115">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="02b39-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="02b39-116">Spécifie les tailles minimale et maximale que les messages entrants doivent être pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="02b39-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="02b39-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="02b39-117">Text value</span></span>

<span data-ttu-id="02b39-118">La valeur de texte est un entier qui identifie la taille maximale du message en octets.</span><span class="sxs-lookup"><span data-stu-id="02b39-118">The text value is an integer that identifies the maximum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="02b39-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="02b39-119">Remarks</span></span>

<span data-ttu-id="02b39-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="02b39-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02b39-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="02b39-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02b39-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="02b39-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="02b39-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="02b39-123">Schema Name</span></span>  <br/> |<span data-ttu-id="02b39-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="02b39-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="02b39-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="02b39-125">Validation File</span></span>  <br/> |<span data-ttu-id="02b39-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="02b39-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02b39-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="02b39-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="02b39-128">True</span><span class="sxs-lookup"><span data-stu-id="02b39-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02b39-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="02b39-129">See also</span></span>



[<span data-ttu-id="02b39-130">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="02b39-130">MinimumSize</span></span>](minimumsize.md)


- [<span data-ttu-id="02b39-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="02b39-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

