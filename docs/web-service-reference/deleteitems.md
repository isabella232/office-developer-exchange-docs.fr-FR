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
description: L’élément DeleteItems indique les éléments dans un dossier un utilisateur est autorisé à supprimer. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 0be2154d1ceb6a995df8b27033fdc59bca81f9ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755878"
---
# <a name="deleteitems"></a><span data-ttu-id="9b538-104">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="9b538-104">DeleteItems</span></span>

<span data-ttu-id="9b538-105">L’élément **DeleteItems** indique les éléments dans un dossier un utilisateur est autorisé à supprimer.</span><span class="sxs-lookup"><span data-stu-id="9b538-105">The **DeleteItems** element indicates which items in a folder a user has permission to delete.</span></span> <span data-ttu-id="9b538-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9b538-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 <span data-ttu-id="9b538-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="9b538-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b538-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9b538-108">Attributes and elements</span></span>

<span data-ttu-id="9b538-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9b538-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b538-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="9b538-110">Attributes</span></span>

<span data-ttu-id="9b538-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9b538-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b538-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9b538-112">Child elements</span></span>

<span data-ttu-id="9b538-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9b538-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9b538-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9b538-114">Parent elements</span></span>

|<span data-ttu-id="9b538-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9b538-115">**Element**</span></span>|<span data-ttu-id="9b538-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="9b538-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b538-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="9b538-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="9b538-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="9b538-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9b538-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="9b538-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="9b538-p104">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="9b538-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9b538-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9b538-123">Text value</span></span>

<span data-ttu-id="9b538-124">Le tableau suivant répertorie les valeurs possibles pour l’élément **DeleteItems** .</span><span class="sxs-lookup"><span data-stu-id="9b538-124">The following table lists the possible values for the **DeleteItems** element.</span></span> 
  
<span data-ttu-id="9b538-125">**Valeurs de texte des éléments DeleteItems**</span><span class="sxs-lookup"><span data-stu-id="9b538-125">**DeleteItems element text values**</span></span>

|<span data-ttu-id="9b538-126">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="9b538-126">**Value**</span></span>|<span data-ttu-id="9b538-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="9b538-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9b538-128">None</span><span class="sxs-lookup"><span data-stu-id="9b538-128">None</span></span>  <br/> |<span data-ttu-id="9b538-129">Indique que l’utilisateur n’est pas autorisé à supprimer des éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="9b538-129">Indicates that the user does not have permission to delete items in the folder.</span></span>  <br/> |
|<span data-ttu-id="9b538-130">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="9b538-130">Owned</span></span>  <br/> |<span data-ttu-id="9b538-131">Indique que l’utilisateur est autorisé à supprimer les éléments qui appartiennent à l’utilisateur dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="9b538-131">Indicates that the user has permission to delete the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="9b538-132">Tous</span><span class="sxs-lookup"><span data-stu-id="9b538-132">All</span></span>  <br/> |<span data-ttu-id="9b538-133">Indique que l’utilisateur est autorisé à supprimer tous les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="9b538-133">Indicates that the user has permission to delete all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b538-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="9b538-134">Remarks</span></span>

<span data-ttu-id="9b538-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9b538-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b538-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9b538-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b538-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9b538-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b538-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9b538-138">Schema Name</span></span>  <br/> |<span data-ttu-id="9b538-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9b538-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b538-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9b538-140">Validation File</span></span>  <br/> |<span data-ttu-id="9b538-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9b538-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b538-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9b538-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b538-143">False</span><span class="sxs-lookup"><span data-stu-id="9b538-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b538-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9b538-144">See also</span></span>

- [<span data-ttu-id="9b538-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9b538-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="9b538-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="9b538-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

