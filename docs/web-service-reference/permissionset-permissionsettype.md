---
title: PermissionSet (PermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d
description: L’élément PermissionSet contient toutes les autorisations configurées pour un dossier.
ms.openlocfilehash: 5639ee8ba64742f39c0274f4e3aaa76d75bea42b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468130"
---
# <a name="permissionset-permissionsettype"></a><span data-ttu-id="9adb3-103">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="9adb3-103">PermissionSet (PermissionSetType)</span></span>

<span data-ttu-id="9adb3-104">L’élément **PermissionSet** contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="9adb3-104">The **PermissionSet** element contains all the permissions that are configured for a folder.</span></span> 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="9adb3-105">**PermissionSetType**</span><span class="sxs-lookup"><span data-stu-id="9adb3-105">**PermissionSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9adb3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9adb3-106">Attributes and elements</span></span>

<span data-ttu-id="9adb3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9adb3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9adb3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9adb3-108">Attributes</span></span>

<span data-ttu-id="9adb3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9adb3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9adb3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9adb3-110">Child elements</span></span>

|<span data-ttu-id="9adb3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9adb3-111">**Element**</span></span>|<span data-ttu-id="9adb3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9adb3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9adb3-113">Autorisations</span><span class="sxs-lookup"><span data-stu-id="9adb3-113">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="9adb3-114">Contient la collection d’autorisations pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="9adb3-114">Contains the collection of permissions for a folder.</span></span> <span data-ttu-id="9adb3-115">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="9adb3-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="9adb3-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="9adb3-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="9adb3-117">Contient un tableau d’entrées inconnues qui ne peuvent pas être résolues par rapport au service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9adb3-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="9adb3-118">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="9adb3-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9adb3-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9adb3-119">Parent elements</span></span>

|<span data-ttu-id="9adb3-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9adb3-120">**Element**</span></span>|<span data-ttu-id="9adb3-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="9adb3-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9adb3-122">Folder</span><span class="sxs-lookup"><span data-stu-id="9adb3-122">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="9adb3-123">Définit un dossier à créer, obtenir, Rechercher, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="9adb3-123">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="9adb3-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="9adb3-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="9adb3-125">Représente un dossier de recherche contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9adb3-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9adb3-126">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="9adb3-126">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="9adb3-127">Représente un dossier de contacts contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9adb3-127">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9adb3-128">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="9adb3-128">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="9adb3-129">Représente un dossier tâches contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9adb3-129">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9adb3-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="9adb3-130">Remarks</span></span>

<span data-ttu-id="9adb3-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9adb3-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="9adb3-132">Cet élément a été introduit dans Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9adb3-132">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="9adb3-133">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="9adb3-133">Version differences</span></span>

<span data-ttu-id="9adb3-134">Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange à partir d’Exchange 2013, les autorisations de dossiers ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a une valeur de **AllProperties** dans la demande d’opération [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9adb3-134">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="9adb3-135">Pour récupérer les autorisations de dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément [AdditionalProperties](additionalproperties.md) dans la demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="9adb3-135">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9adb3-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9adb3-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9adb3-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9adb3-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9adb3-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9adb3-138">Schema Name</span></span>  <br/> |<span data-ttu-id="9adb3-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9adb3-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="9adb3-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9adb3-140">Validation File</span></span>  <br/> |<span data-ttu-id="9adb3-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9adb3-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9adb3-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9adb3-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="9adb3-143">False</span><span class="sxs-lookup"><span data-stu-id="9adb3-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9adb3-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9adb3-144">See also</span></span>



- [<span data-ttu-id="9adb3-145">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9adb3-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9adb3-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="9adb3-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

