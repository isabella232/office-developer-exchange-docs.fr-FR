---
title: Modifier les éléments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EditItems
api_type:
- schema
ms.assetid: 1cb14493-c999-4d66-b82c-ecb410dc1c00
description: L’élément de modifier les éléments indique les éléments dans un dossier un utilisateur est autorisé à modifier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: bbcc103f171cca7c72967796284c6016d8e284e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756084"
---
# <a name="edititems"></a><span data-ttu-id="b7863-104">Modifier les éléments</span><span class="sxs-lookup"><span data-stu-id="b7863-104">EditItems</span></span>

<span data-ttu-id="b7863-105">L’élément de **Modifier les éléments** indique les éléments dans un dossier un utilisateur est autorisé à modifier.</span><span class="sxs-lookup"><span data-stu-id="b7863-105">The **EditItems** element indicates which items in a folder a user has permission to edit.</span></span> <span data-ttu-id="b7863-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b7863-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<EditItems>None or Owned or All</EditItems>
```

 <span data-ttu-id="b7863-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="b7863-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7863-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b7863-108">Attributes and elements</span></span>

<span data-ttu-id="b7863-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b7863-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7863-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="b7863-110">Attributes</span></span>

<span data-ttu-id="b7863-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b7863-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7863-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b7863-112">Child elements</span></span>

<span data-ttu-id="b7863-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b7863-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7863-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b7863-114">Parent elements</span></span>

|<span data-ttu-id="b7863-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b7863-115">**Element**</span></span>|<span data-ttu-id="b7863-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="b7863-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7863-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="b7863-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="b7863-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="b7863-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="b7863-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="b7863-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="b7863-p104">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="b7863-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b7863-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b7863-123">Text value</span></span>

<span data-ttu-id="b7863-124">Le tableau suivant répertorie les valeurs possibles pour l’élément de **Modifier les éléments** .</span><span class="sxs-lookup"><span data-stu-id="b7863-124">The following table lists the possible values for the **EditItems** element.</span></span> 
  
<span data-ttu-id="b7863-125">**Valeurs de texte d’élément modifier les éléments**</span><span class="sxs-lookup"><span data-stu-id="b7863-125">**EditItems element text values**</span></span>

|<span data-ttu-id="b7863-126">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="b7863-126">**Value**</span></span>|<span data-ttu-id="b7863-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="b7863-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b7863-128">None</span><span class="sxs-lookup"><span data-stu-id="b7863-128">None</span></span>  <br/> |<span data-ttu-id="b7863-129">Indique que l’utilisateur n’est pas autorisé à modifier des éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="b7863-129">Indicates that the user does not have permission to edit items in the folder.</span></span>  <br/> |
|<span data-ttu-id="b7863-130">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="b7863-130">Owned</span></span>  <br/> |<span data-ttu-id="b7863-131">Indique que l’utilisateur est autorisé à modifier les éléments qui appartiennent à l’utilisateur dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="b7863-131">Indicates that the user has permission to edit the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="b7863-132">Tous</span><span class="sxs-lookup"><span data-stu-id="b7863-132">All</span></span>  <br/> |<span data-ttu-id="b7863-133">Indique que l’utilisateur est autorisé à modifier tous les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="b7863-133">Indicates that the user has permission to edit all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b7863-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="b7863-134">Remarks</span></span>

<span data-ttu-id="b7863-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b7863-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7863-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b7863-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7863-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b7863-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b7863-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b7863-138">Schema Name</span></span>  <br/> |<span data-ttu-id="b7863-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b7863-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="b7863-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b7863-140">Validation File</span></span>  <br/> |<span data-ttu-id="b7863-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b7863-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b7863-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b7863-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="b7863-143">False</span><span class="sxs-lookup"><span data-stu-id="b7863-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b7863-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b7863-144">See also</span></span>

- [<span data-ttu-id="b7863-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7863-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="b7863-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="b7863-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

