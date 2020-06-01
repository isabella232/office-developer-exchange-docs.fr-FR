---
title: UnknownEntries
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownEntries
api_type:
- schema
ms.assetid: 107ec73e-083a-4956-9d37-33d4734cc157
description: L’élément UnknownEntries contient un tableau d’entrées d’autorisation inconnues qui ne peuvent pas être résolues sur le service d’annuaire Active Directory. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 68cb2518b895ca0a74e6b9ed649ee92b7502ab05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459418"
---
# <a name="unknownentries"></a><span data-ttu-id="f0680-104">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="f0680-104">UnknownEntries</span></span>

<span data-ttu-id="f0680-105">L’élément **UnknownEntries** contient un tableau d’entrées d’autorisation inconnues qui ne peuvent pas être résolues sur le service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0680-105">The **UnknownEntries** element contains an array of unknown permission entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="f0680-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f0680-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntries>
   <UnknownEntry/>
</UnknownEntries>
```

 <span data-ttu-id="f0680-107">**ArrayOfUnknownEntriesType**</span><span class="sxs-lookup"><span data-stu-id="f0680-107">**ArrayOfUnknownEntriesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0680-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f0680-108">Attributes and elements</span></span>

<span data-ttu-id="f0680-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f0680-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0680-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="f0680-110">Attributes</span></span>

<span data-ttu-id="f0680-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f0680-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0680-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f0680-112">Child elements</span></span>

|<span data-ttu-id="f0680-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f0680-113">**Element**</span></span>|<span data-ttu-id="f0680-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f0680-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0680-115">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="f0680-115">UnknownEntry</span></span>](unknownentry.md) <br/> |<span data-ttu-id="f0680-116">Représente une entrée d’autorisation inconnue unique qui ne peut pas être résolue par rapport à Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0680-116">Represents a single unknown permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="f0680-117">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f0680-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0680-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f0680-118">Parent elements</span></span>

|<span data-ttu-id="f0680-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f0680-119">**Element**</span></span>|<span data-ttu-id="f0680-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="f0680-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0680-121">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="f0680-121">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="f0680-122">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="f0680-122">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="f0680-123">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f0680-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f0680-124">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="f0680-124">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="f0680-125">Contient toutes les autorisations configurées pour un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="f0680-125">Contains all the permissions that are configured for a calendar folder.</span></span> <span data-ttu-id="f0680-126">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f0680-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f0680-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="f0680-127">Remarks</span></span>

<span data-ttu-id="f0680-128">Vous pouvez supprimer des entrées inconnues d’un dossier à l’aide de l’opération UpdateFolder avec l’élément [SetFolderField](setfolderfield.md) .</span><span class="sxs-lookup"><span data-stu-id="f0680-128">You can delete unknown entries from a folder by using the UpdateFolder operation with the [SetFolderField](setfolderfield.md) element.</span></span> <span data-ttu-id="f0680-129">Les entrées inconnues sont supprimées lorsque vous réinitialisez le PermissionSet à l’aide de l’option SetFolderField de l’opération UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="f0680-129">The unknown entries are deleted when you reset the PermissionSet by using the SetFolderField option of the UpdateFolder operation.</span></span> <span data-ttu-id="f0680-130">Les services Web Exchange ne prennent pas en charge la suppression d’entrées individuelles.</span><span class="sxs-lookup"><span data-stu-id="f0680-130">Exchange Web Services does not support the deletion of individual entries.</span></span> 
  
<span data-ttu-id="f0680-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f0680-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0680-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f0680-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0680-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f0680-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f0680-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f0680-134">Schema Name</span></span>  <br/> |<span data-ttu-id="f0680-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f0680-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="f0680-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f0680-136">Validation File</span></span>  <br/> |<span data-ttu-id="f0680-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f0680-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f0680-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f0680-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0680-139">False</span><span class="sxs-lookup"><span data-stu-id="f0680-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0680-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f0680-140">See also</span></span>



[<span data-ttu-id="f0680-141">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="f0680-141">UpdateFolder operation</span></span>](updatefolder-operation.md)


- [<span data-ttu-id="f0680-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f0680-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f0680-143">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="f0680-143">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

