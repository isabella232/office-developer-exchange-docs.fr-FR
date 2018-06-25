---
title: PlayOnPhone (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 206a2ad1-a01d-4e71-99a1-90c2530423da
description: L’élément PlayOnPhone définit une demande pour lire un élément sur un téléphone.
ms.openlocfilehash: 7e5c1e25512a59d1ac3295b476fcc2b6b0f5a2b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828825"
---
# <a name="playonphone-um-web-service"></a><span data-ttu-id="d9a18-103">PlayOnPhone (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d9a18-103">PlayOnPhone (UM web service)</span></span>

<span data-ttu-id="d9a18-104">L’élément **PlayOnPhone** définit une demande pour lire un élément sur un téléphone.</span><span class="sxs-lookup"><span data-stu-id="d9a18-104">The **PlayOnPhone** element defines a request to play an item on a telephone.</span></span> 
  
[<span data-ttu-id="d9a18-105">PlayOnPhone (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d9a18-105">PlayOnPhone (UM web service)</span></span>](playonphone-um-web-service.md)
  
```xml
<PlayOnPhone>
  <entryId>   </entryId>
  <DialString>   </DialString>
</PlayOnPhone>
```

 <span data-ttu-id="d9a18-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="d9a18-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9a18-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d9a18-107">Attributes and elements</span></span>

<span data-ttu-id="d9a18-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d9a18-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9a18-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="d9a18-109">Attributes</span></span>

<span data-ttu-id="d9a18-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d9a18-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9a18-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d9a18-111">Child elements</span></span>

|<span data-ttu-id="d9a18-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d9a18-112">**Element**</span></span>|<span data-ttu-id="d9a18-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="d9a18-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9a18-114">propriété entryId (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d9a18-114">entryId (UM web service)</span></span>](entryid-um-web-service.md) <br/> |<span data-ttu-id="d9a18-115">Contient la valeur qui représente l’identificateur de l’élément à lire sur le téléphone dans une requête [d’opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="d9a18-115">Contains the value that represents the identifier of the item to play on the telephone in a [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) request.</span></span>  <br/> |
|[<span data-ttu-id="d9a18-116">dialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d9a18-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="d9a18-117">Contient la valeur du numéro de téléphone à composer.</span><span class="sxs-lookup"><span data-stu-id="d9a18-117">Contains the value for the telephone number to dial.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d9a18-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d9a18-118">Parent elements</span></span>

<span data-ttu-id="d9a18-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d9a18-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d9a18-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d9a18-120">Text value</span></span>

<span data-ttu-id="d9a18-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d9a18-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9a18-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d9a18-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9a18-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d9a18-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d9a18-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d9a18-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d9a18-125">Messages</span><span class="sxs-lookup"><span data-stu-id="d9a18-125">Messages</span></span>  <br/> |
|<span data-ttu-id="d9a18-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d9a18-126">Validation File</span></span>  <br/> |<span data-ttu-id="d9a18-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d9a18-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d9a18-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d9a18-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9a18-129">False</span><span class="sxs-lookup"><span data-stu-id="d9a18-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9a18-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d9a18-130">See also</span></span>



[<span data-ttu-id="d9a18-131">Opération PlayOnPhone (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d9a18-131">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)

