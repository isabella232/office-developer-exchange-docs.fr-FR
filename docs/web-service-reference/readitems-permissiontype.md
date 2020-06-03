---
title: ReadItems (PermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: 0a11a802-28e2-436b-b5a9-30fd064675a6
description: L’élément ReadItems indique si un utilisateur est autorisé à lire des éléments dans un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: af6ef5107b5e4f2b3071c0bc9b4b528efea6dcca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468270"
---
# <a name="readitems-permissiontype"></a><span data-ttu-id="5bc60-104">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="5bc60-104">ReadItems (PermissionType)</span></span>

<span data-ttu-id="5bc60-105">L’élément **ReadItems** indique si un utilisateur est autorisé à lire des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="5bc60-105">The **ReadItems** element indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="5bc60-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5bc60-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or FullDetails</ReadItems>
```

 <span data-ttu-id="5bc60-107">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="5bc60-107">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5bc60-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5bc60-108">Attributes and elements</span></span>

<span data-ttu-id="5bc60-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5bc60-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5bc60-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="5bc60-110">Attributes</span></span>

<span data-ttu-id="5bc60-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5bc60-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5bc60-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5bc60-112">Child elements</span></span>

<span data-ttu-id="5bc60-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5bc60-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5bc60-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5bc60-114">Parent elements</span></span>

|<span data-ttu-id="5bc60-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5bc60-115">**Element**</span></span>|<span data-ttu-id="5bc60-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="5bc60-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bc60-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="5bc60-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="5bc60-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="5bc60-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5bc60-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5bc60-120">Text value</span></span>

<span data-ttu-id="5bc60-121">Le tableau suivant répertorie les valeurs possibles pour l’élément **ReadItems** .</span><span class="sxs-lookup"><span data-stu-id="5bc60-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="5bc60-122">**Valeurs de texte de l’élément ReadItems**</span><span class="sxs-lookup"><span data-stu-id="5bc60-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="5bc60-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="5bc60-123">**Value**</span></span>|<span data-ttu-id="5bc60-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="5bc60-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5bc60-125">Aucun</span><span class="sxs-lookup"><span data-stu-id="5bc60-125">None</span></span>  <br/> |<span data-ttu-id="5bc60-126">Indique que l’utilisateur n’est pas autorisé à lire les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="5bc60-126">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="5bc60-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="5bc60-127">FullDetails</span></span>  <br/> |<span data-ttu-id="5bc60-128">Indique que l’utilisateur est autorisé à lire tous les éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="5bc60-128">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5bc60-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="5bc60-129">Remarks</span></span>

<span data-ttu-id="5bc60-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5bc60-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5bc60-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5bc60-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5bc60-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5bc60-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5bc60-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5bc60-133">Schema Name</span></span>  <br/> |<span data-ttu-id="5bc60-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5bc60-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="5bc60-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5bc60-135">Validation File</span></span>  <br/> |<span data-ttu-id="5bc60-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5bc60-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5bc60-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5bc60-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="5bc60-138">False</span><span class="sxs-lookup"><span data-stu-id="5bc60-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5bc60-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5bc60-139">See also</span></span>



- [<span data-ttu-id="5bc60-140">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5bc60-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5bc60-141">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="5bc60-141">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

