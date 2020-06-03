---
title: EditItems
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
description: L’élément EditItems indique les éléments d’un dossier qu’un utilisateur est autorisé à modifier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 0c3800b4d242dccb7455e0d0dea74e766db22854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459250"
---
# <a name="edititems"></a><span data-ttu-id="327fa-104">EditItems</span><span class="sxs-lookup"><span data-stu-id="327fa-104">EditItems</span></span>

<span data-ttu-id="327fa-105">L’élément **EditItems** indique les éléments d’un dossier qu’un utilisateur est autorisé à modifier.</span><span class="sxs-lookup"><span data-stu-id="327fa-105">The **EditItems** element indicates which items in a folder a user has permission to edit.</span></span> <span data-ttu-id="327fa-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="327fa-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<EditItems>None or Owned or All</EditItems>
```

 <span data-ttu-id="327fa-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="327fa-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="327fa-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="327fa-108">Attributes and elements</span></span>

<span data-ttu-id="327fa-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="327fa-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="327fa-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="327fa-110">Attributes</span></span>

<span data-ttu-id="327fa-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="327fa-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="327fa-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="327fa-112">Child elements</span></span>

<span data-ttu-id="327fa-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="327fa-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="327fa-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="327fa-114">Parent elements</span></span>

|<span data-ttu-id="327fa-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="327fa-115">**Element**</span></span>|<span data-ttu-id="327fa-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="327fa-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="327fa-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="327fa-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="327fa-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="327fa-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="327fa-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="327fa-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="327fa-p104">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="327fa-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="327fa-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="327fa-123">Text value</span></span>

<span data-ttu-id="327fa-124">Le tableau suivant répertorie les valeurs possibles pour l’élément **EditItems** .</span><span class="sxs-lookup"><span data-stu-id="327fa-124">The following table lists the possible values for the **EditItems** element.</span></span> 
  
<span data-ttu-id="327fa-125">**Valeurs de texte de l’élément EditItems**</span><span class="sxs-lookup"><span data-stu-id="327fa-125">**EditItems element text values**</span></span>

|<span data-ttu-id="327fa-126">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="327fa-126">**Value**</span></span>|<span data-ttu-id="327fa-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="327fa-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="327fa-128">Aucun</span><span class="sxs-lookup"><span data-stu-id="327fa-128">None</span></span>  <br/> |<span data-ttu-id="327fa-129">Indique que l’utilisateur n’est pas autorisé à modifier les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="327fa-129">Indicates that the user does not have permission to edit items in the folder.</span></span>  <br/> |
|<span data-ttu-id="327fa-130">Appartien</span><span class="sxs-lookup"><span data-stu-id="327fa-130">Owned</span></span>  <br/> |<span data-ttu-id="327fa-131">Indique que l’utilisateur est autorisé à modifier les éléments dont il est propriétaire dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="327fa-131">Indicates that the user has permission to edit the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="327fa-132">Tous</span><span class="sxs-lookup"><span data-stu-id="327fa-132">All</span></span>  <br/> |<span data-ttu-id="327fa-133">Indique que l’utilisateur est autorisé à modifier tous les éléments du dossier.</span><span class="sxs-lookup"><span data-stu-id="327fa-133">Indicates that the user has permission to edit all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="327fa-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="327fa-134">Remarks</span></span>

<span data-ttu-id="327fa-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="327fa-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="327fa-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="327fa-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="327fa-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="327fa-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="327fa-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="327fa-138">Schema Name</span></span>  <br/> |<span data-ttu-id="327fa-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="327fa-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="327fa-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="327fa-140">Validation File</span></span>  <br/> |<span data-ttu-id="327fa-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="327fa-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="327fa-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="327fa-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="327fa-143">False</span><span class="sxs-lookup"><span data-stu-id="327fa-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="327fa-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="327fa-144">See also</span></span>

- [<span data-ttu-id="327fa-145">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="327fa-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="327fa-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="327fa-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

