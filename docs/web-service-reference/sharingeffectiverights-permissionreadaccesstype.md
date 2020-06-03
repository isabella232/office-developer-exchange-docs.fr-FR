---
title: SharingEffectiveRights (PermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: 808bb4a1-aa2d-48c5-94b3-551b52c348bd
description: L’élément SharingEffectiveRights indique les autorisations dont dispose l’utilisateur pour les données de contact partagées.
ms.openlocfilehash: 64b1e6d831068e9699e9cd47693e74919e0416a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526661"
---
# <a name="sharingeffectiverights-permissionreadaccesstype"></a><span data-ttu-id="ea2f1-103">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="ea2f1-103">SharingEffectiveRights (PermissionReadAccessType)</span></span>

<span data-ttu-id="ea2f1-104">L’élément **SharingEffectiveRights** indique les autorisations dont dispose l’utilisateur pour les données de contact partagées.</span><span class="sxs-lookup"><span data-stu-id="ea2f1-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the contact data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | FullDetails</SharingEffectiveRights >
```

 <span data-ttu-id="ea2f1-105">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="ea2f1-105">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea2f1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ea2f1-106">Attributes and elements</span></span>

<span data-ttu-id="ea2f1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ea2f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea2f1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ea2f1-108">Attributes</span></span>

<span data-ttu-id="ea2f1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ea2f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea2f1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ea2f1-110">Child elements</span></span>

<span data-ttu-id="ea2f1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ea2f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea2f1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ea2f1-112">Parent elements</span></span>

|<span data-ttu-id="ea2f1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ea2f1-113">**Element**</span></span>|<span data-ttu-id="ea2f1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea2f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea2f1-115">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="ea2f1-115">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="ea2f1-116">Représente un dossier de contacts contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ea2f1-116">Represents a Contacts folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea2f1-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ea2f1-117">Text value</span></span>

<span data-ttu-id="ea2f1-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **SharingEffectiveRights** .</span><span class="sxs-lookup"><span data-stu-id="ea2f1-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
<span data-ttu-id="ea2f1-119">**Valeurs de texte de l’élément SharingEffectiveRights**</span><span class="sxs-lookup"><span data-stu-id="ea2f1-119">**SharingEffectiveRights element text values**</span></span>

|<span data-ttu-id="ea2f1-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="ea2f1-120">**Value**</span></span>|<span data-ttu-id="ea2f1-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea2f1-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea2f1-122">Aucun</span><span class="sxs-lookup"><span data-stu-id="ea2f1-122">None</span></span>  <br/> |<span data-ttu-id="ea2f1-123">Indique que l’utilisateur n’est pas autorisé à lire les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="ea2f1-123">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="ea2f1-124">FullDetails</span><span class="sxs-lookup"><span data-stu-id="ea2f1-124">FullDetails</span></span>  <br/> |<span data-ttu-id="ea2f1-125">Indique que l’utilisateur est autorisé à lire tous les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="ea2f1-125">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ea2f1-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="ea2f1-126">Remarks</span></span>

<span data-ttu-id="ea2f1-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ea2f1-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea2f1-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ea2f1-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea2f1-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ea2f1-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea2f1-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ea2f1-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ea2f1-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ea2f1-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ea2f1-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ea2f1-132">Validation File</span></span>  <br/> |<span data-ttu-id="ea2f1-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea2f1-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea2f1-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ea2f1-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea2f1-135">False</span><span class="sxs-lookup"><span data-stu-id="ea2f1-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea2f1-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ea2f1-136">See also</span></span>



- [<span data-ttu-id="ea2f1-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ea2f1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

