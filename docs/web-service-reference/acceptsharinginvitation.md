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
description: L’élément AcceptSharingInvitation est utilisé pour accepter une invitation qui autorise l’accès au calendrier ou aux données de contacts d’un autre utilisateur.
ms.openlocfilehash: c8cdae707bd122e74fa0e284163d1540d857c3de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461708"
---
# <a name="acceptsharinginvitation"></a><span data-ttu-id="8b49f-103">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="8b49f-103">AcceptSharingInvitation</span></span>

<span data-ttu-id="8b49f-104">L’élément **AcceptSharingInvitation** est utilisé pour accepter une invitation qui autorise l’accès au calendrier ou aux données de contacts d’un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8b49f-104">The **AcceptSharingInvitation** element is used to accept an invitation that allows access to another user's calendar or contacts data.</span></span> 
  
```xml
<AcceptSharingInvitation>
   <ReferenceItemId/>
</AcceptSharingInvitation>
```

 <span data-ttu-id="8b49f-105">**AcceptSharingInvitationType**</span><span class="sxs-lookup"><span data-stu-id="8b49f-105">**AcceptSharingInvitationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b49f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8b49f-106">Attributes and elements</span></span>

<span data-ttu-id="8b49f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8b49f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b49f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8b49f-108">Attributes</span></span>

<span data-ttu-id="8b49f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8b49f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b49f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8b49f-110">Child elements</span></span>

|<span data-ttu-id="8b49f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8b49f-111">**Element**</span></span>|<span data-ttu-id="8b49f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8b49f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b49f-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="8b49f-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="8b49f-114">Identifie l’élément auquel l’objet de réponse fait référence.</span><span class="sxs-lookup"><span data-stu-id="8b49f-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b49f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8b49f-115">Parent elements</span></span>

|<span data-ttu-id="8b49f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8b49f-116">**Element**</span></span>|<span data-ttu-id="8b49f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="8b49f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b49f-118">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="8b49f-118">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="8b49f-119">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b49f-119">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8b49f-120">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="8b49f-120">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="8b49f-121">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="8b49f-121">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8b49f-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="8b49f-122">Remarks</span></span>

<span data-ttu-id="8b49f-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b49f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b49f-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8b49f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b49f-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8b49f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b49f-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8b49f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="8b49f-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8b49f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b49f-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8b49f-128">Validation File</span></span>  <br/> |<span data-ttu-id="8b49f-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b49f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b49f-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8b49f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b49f-131">False</span><span class="sxs-lookup"><span data-stu-id="8b49f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b49f-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8b49f-132">See also</span></span>

- [<span data-ttu-id="8b49f-133">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="8b49f-133">CreateItem (AcceptSharingInvitation)</span></span>](createitem-acceptsharinginvitation.md)
- [<span data-ttu-id="8b49f-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8b49f-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

