---
title: AcceptSharingInvitation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AcceptSharingInvitation
api_type:
- schema
ms.assetid: 3c2a47d6-490d-425b-8893-089a4f8882cd
description: L’élément AcceptSharingInvitation est utilisé pour accepter une invitation qui permet d’accéder aux données de contacts ou de calendrier d’un autre utilisateur.
ms.openlocfilehash: 06439739e6cc544d5039ac9d18e0452b1d42a0ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756307"
---
# <a name="acceptsharinginvitation"></a><span data-ttu-id="40443-103">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="40443-103">AcceptSharingInvitation</span></span>

<span data-ttu-id="40443-104">L’élément **AcceptSharingInvitation** est utilisé pour accepter une invitation qui permet d’accéder aux données de contacts ou de calendrier d’un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="40443-104">The **AcceptSharingInvitation** element is used to accept an invitation that allows access to another user's calendar or contacts data.</span></span> 
  
```xml
<AcceptSharingInvitation>
   <ReferenceItemId/>
</AcceptSharingInvitation>
```

 <span data-ttu-id="40443-105">**AcceptSharingInvitationType**</span><span class="sxs-lookup"><span data-stu-id="40443-105">**AcceptSharingInvitationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40443-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="40443-106">Attributes and elements</span></span>

<span data-ttu-id="40443-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="40443-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40443-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="40443-108">Attributes</span></span>

<span data-ttu-id="40443-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="40443-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40443-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="40443-110">Child elements</span></span>

|<span data-ttu-id="40443-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="40443-111">**Element**</span></span>|<span data-ttu-id="40443-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="40443-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40443-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="40443-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="40443-114">Identifie l’élément auquel fait référence l’objet de réponse.</span><span class="sxs-lookup"><span data-stu-id="40443-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="40443-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="40443-115">Parent elements</span></span>

|<span data-ttu-id="40443-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="40443-116">**Element**</span></span>|<span data-ttu-id="40443-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="40443-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40443-118">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="40443-118">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="40443-119">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="40443-119">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="40443-120">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="40443-120">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="40443-121">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="40443-121">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="40443-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="40443-122">Remarks</span></span>

<span data-ttu-id="40443-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="40443-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40443-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="40443-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40443-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="40443-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="40443-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="40443-126">Schema Name</span></span>  <br/> |<span data-ttu-id="40443-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="40443-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="40443-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="40443-128">Validation File</span></span>  <br/> |<span data-ttu-id="40443-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="40443-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="40443-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="40443-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="40443-131">False</span><span class="sxs-lookup"><span data-stu-id="40443-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40443-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="40443-132">See also</span></span>

- [<span data-ttu-id="40443-133">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="40443-133">CreateItem (AcceptSharingInvitation)</span></span>](createitem-acceptsharinginvitation.md)
- [<span data-ttu-id="40443-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="40443-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

