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
description: L’élément SharingEffectiveRights indique les autorisations dont dispose l’utilisateur pour les données de contact qui sont partagées.
ms.openlocfilehash: 19e67827dd2dbff6fb70423980d670da5cc257a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829486"
---
# <a name="sharingeffectiverights-permissionreadaccesstype"></a><span data-ttu-id="8283c-103">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="8283c-103">SharingEffectiveRights (PermissionReadAccessType)</span></span>

<span data-ttu-id="8283c-104">L’élément **SharingEffectiveRights** indique les autorisations dont dispose l’utilisateur pour les données de contact qui sont partagées.</span><span class="sxs-lookup"><span data-stu-id="8283c-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the contact data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | FullDetails</SharingEffectiveRights >
```

 <span data-ttu-id="8283c-105">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="8283c-105">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8283c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8283c-106">Attributes and elements</span></span>

<span data-ttu-id="8283c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8283c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8283c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8283c-108">Attributes</span></span>

<span data-ttu-id="8283c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8283c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8283c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8283c-110">Child elements</span></span>

<span data-ttu-id="8283c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8283c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8283c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8283c-112">Parent elements</span></span>

|<span data-ttu-id="8283c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8283c-113">**Element**</span></span>|<span data-ttu-id="8283c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="8283c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8283c-115">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="8283c-115">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="8283c-116">Représente un dossier de Contacts qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8283c-116">Represents a Contacts folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8283c-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8283c-117">Text value</span></span>

<span data-ttu-id="8283c-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **SharingEffectiveRights** .</span><span class="sxs-lookup"><span data-stu-id="8283c-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
<span data-ttu-id="8283c-119">**Valeurs de texte des éléments SharingEffectiveRights**</span><span class="sxs-lookup"><span data-stu-id="8283c-119">**SharingEffectiveRights element text values**</span></span>

|<span data-ttu-id="8283c-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="8283c-120">**Value**</span></span>|<span data-ttu-id="8283c-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="8283c-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8283c-122">None</span><span class="sxs-lookup"><span data-stu-id="8283c-122">None</span></span>  <br/> |<span data-ttu-id="8283c-123">Indique que l’utilisateur n’est pas autorisé à lire les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="8283c-123">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="8283c-124">FullDetails</span><span class="sxs-lookup"><span data-stu-id="8283c-124">FullDetails</span></span>  <br/> |<span data-ttu-id="8283c-125">Indique que l’utilisateur est autorisé à lire tous les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="8283c-125">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8283c-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="8283c-126">Remarks</span></span>

<span data-ttu-id="8283c-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8283c-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8283c-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8283c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8283c-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8283c-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8283c-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8283c-130">Schema Name</span></span>  <br/> |<span data-ttu-id="8283c-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8283c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="8283c-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8283c-132">Validation File</span></span>  <br/> |<span data-ttu-id="8283c-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8283c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8283c-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8283c-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="8283c-135">False</span><span class="sxs-lookup"><span data-stu-id="8283c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8283c-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8283c-136">See also</span></span>



- [<span data-ttu-id="8283c-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8283c-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

