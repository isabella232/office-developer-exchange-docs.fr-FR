---
title: GetRooms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 82a737c7-da41-4777-8ad8-89851a0b602b
description: L’élément GetRooms est l’élément racine dans une demande pour obtenir une liste de salles dans une liste de salles particulière.
ms.openlocfilehash: 77fde5980a03d4c0509344933b0901cb21ab7197
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458592"
---
# <a name="getrooms"></a><span data-ttu-id="12c21-103">GetRooms</span><span class="sxs-lookup"><span data-stu-id="12c21-103">GetRooms</span></span>

<span data-ttu-id="12c21-104">L’élément **GetRooms** est l’élément racine dans une demande pour obtenir une liste de salles dans une liste de salles particulière.</span><span class="sxs-lookup"><span data-stu-id="12c21-104">The **GetRooms** element is the root element in a request to get a list of rooms within a particular room list.</span></span> 
  
```XML
<GetRooms>
   <RoomList/>
</GetRooms>
```

 <span data-ttu-id="12c21-105">**GetRoomsType**</span><span class="sxs-lookup"><span data-stu-id="12c21-105">**GetRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12c21-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="12c21-106">Attributes and elements</span></span>

<span data-ttu-id="12c21-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="12c21-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12c21-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="12c21-108">Attributes</span></span>

<span data-ttu-id="12c21-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="12c21-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12c21-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="12c21-110">Child elements</span></span>

|<span data-ttu-id="12c21-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="12c21-111">**Element**</span></span>|<span data-ttu-id="12c21-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="12c21-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12c21-113">RoomList</span><span class="sxs-lookup"><span data-stu-id="12c21-113">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="12c21-114">Représente une adresse de messagerie qui identifie une liste de salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="12c21-114">Represents an e-mail address that identifies a list of meeting rooms</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="12c21-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="12c21-115">Parent elements</span></span>

<span data-ttu-id="12c21-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="12c21-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="12c21-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="12c21-117">Text value</span></span>

<span data-ttu-id="12c21-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="12c21-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="12c21-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="12c21-119">Remarks</span></span>

<span data-ttu-id="12c21-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="12c21-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12c21-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="12c21-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12c21-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="12c21-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="12c21-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="12c21-123">Schema Name</span></span>  <br/> |<span data-ttu-id="12c21-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="12c21-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="12c21-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="12c21-125">Validation File</span></span>  <br/> |<span data-ttu-id="12c21-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="12c21-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="12c21-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="12c21-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="12c21-128">False</span><span class="sxs-lookup"><span data-stu-id="12c21-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12c21-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="12c21-129">See also</span></span>



- [<span data-ttu-id="12c21-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="12c21-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

