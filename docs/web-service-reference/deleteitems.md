---
title: DeleteItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItems
api_type:
- schema
ms.assetid: a5898bfc-f5ae-451d-9713-3e55864c690c
description: L’élément DeleteItems indique les éléments d’un dossier qu’un utilisateur est autorisé à supprimer. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: a0bbefc8b021d047bb2e001669c3e92a6e2536ce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454406"
---
# <a name="deleteitems"></a><span data-ttu-id="86f3d-104">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="86f3d-104">DeleteItems</span></span>

<span data-ttu-id="86f3d-105">L’élément **DeleteItems** indique les éléments d’un dossier qu’un utilisateur est autorisé à supprimer.</span><span class="sxs-lookup"><span data-stu-id="86f3d-105">The **DeleteItems** element indicates which items in a folder a user has permission to delete.</span></span> <span data-ttu-id="86f3d-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="86f3d-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 <span data-ttu-id="86f3d-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="86f3d-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86f3d-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="86f3d-108">Attributes and elements</span></span>

<span data-ttu-id="86f3d-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="86f3d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86f3d-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="86f3d-110">Attributes</span></span>

<span data-ttu-id="86f3d-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="86f3d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86f3d-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="86f3d-112">Child elements</span></span>

<span data-ttu-id="86f3d-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="86f3d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="86f3d-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="86f3d-114">Parent elements</span></span>

|<span data-ttu-id="86f3d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="86f3d-115">**Element**</span></span>|<span data-ttu-id="86f3d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="86f3d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86f3d-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="86f3d-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="86f3d-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="86f3d-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="86f3d-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="86f3d-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="86f3d-p104">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="86f3d-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="86f3d-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="86f3d-123">Text value</span></span>

<span data-ttu-id="86f3d-124">Le tableau suivant répertorie les valeurs possibles pour l’élément **DeleteItems** .</span><span class="sxs-lookup"><span data-stu-id="86f3d-124">The following table lists the possible values for the **DeleteItems** element.</span></span> 
  
<span data-ttu-id="86f3d-125">**Valeurs de texte de l’élément DeleteItems**</span><span class="sxs-lookup"><span data-stu-id="86f3d-125">**DeleteItems element text values**</span></span>

|<span data-ttu-id="86f3d-126">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="86f3d-126">**Value**</span></span>|<span data-ttu-id="86f3d-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="86f3d-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="86f3d-128">Aucune</span><span class="sxs-lookup"><span data-stu-id="86f3d-128">None</span></span>  <br/> |<span data-ttu-id="86f3d-129">Indique que l’utilisateur n’est pas autorisé à supprimer des éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="86f3d-129">Indicates that the user does not have permission to delete items in the folder.</span></span>  <br/> |
|<span data-ttu-id="86f3d-130">Appartien</span><span class="sxs-lookup"><span data-stu-id="86f3d-130">Owned</span></span>  <br/> |<span data-ttu-id="86f3d-131">Indique que l’utilisateur est autorisé à supprimer les éléments dont il est propriétaire dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="86f3d-131">Indicates that the user has permission to delete the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="86f3d-132">Tous</span><span class="sxs-lookup"><span data-stu-id="86f3d-132">All</span></span>  <br/> |<span data-ttu-id="86f3d-133">Indique que l’utilisateur est autorisé à supprimer tous les éléments du dossier.</span><span class="sxs-lookup"><span data-stu-id="86f3d-133">Indicates that the user has permission to delete all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="86f3d-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="86f3d-134">Remarks</span></span>

<span data-ttu-id="86f3d-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="86f3d-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86f3d-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="86f3d-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86f3d-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="86f3d-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86f3d-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="86f3d-138">Schema Name</span></span>  <br/> |<span data-ttu-id="86f3d-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="86f3d-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="86f3d-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="86f3d-140">Validation File</span></span>  <br/> |<span data-ttu-id="86f3d-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="86f3d-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="86f3d-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="86f3d-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="86f3d-143">False</span><span class="sxs-lookup"><span data-stu-id="86f3d-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86f3d-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="86f3d-144">See also</span></span>

- [<span data-ttu-id="86f3d-145">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="86f3d-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="86f3d-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="86f3d-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

