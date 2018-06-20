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
description: L’élément PermissionSet contient toutes les autorisations qui sont configurées pour un dossier.
ms.openlocfilehash: 0fa0ac78a0db2bf382ad413cbb8bd072aa88c6fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828732"
---
# <a name="permissionset-permissionsettype"></a><span data-ttu-id="f69f0-103">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="f69f0-103">PermissionSet (PermissionSetType)</span></span>

<span data-ttu-id="f69f0-104">L’élément **PermissionSet** contient toutes les autorisations qui sont configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="f69f0-104">The **PermissionSet** element contains all the permissions that are configured for a folder.</span></span> 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="f69f0-105">**PermissionSetType**</span><span class="sxs-lookup"><span data-stu-id="f69f0-105">**PermissionSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f69f0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f69f0-106">Attributes and elements</span></span>

<span data-ttu-id="f69f0-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f69f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f69f0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f69f0-108">Attributes</span></span>

<span data-ttu-id="f69f0-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f69f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f69f0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f69f0-110">Child elements</span></span>

|<span data-ttu-id="f69f0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f69f0-111">**Element**</span></span>|<span data-ttu-id="f69f0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f69f0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f69f0-113">Autorisations</span><span class="sxs-lookup"><span data-stu-id="f69f0-113">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="f69f0-114">Contient la collection des autorisations pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="f69f0-114">Contains the collection of permissions for a folder.</span></span> <span data-ttu-id="f69f0-115">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f69f0-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f69f0-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="f69f0-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="f69f0-117">Contient un tableau d’entrées inconnus qui ne peut pas être résolu sur le service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f69f0-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="f69f0-118">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f69f0-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f69f0-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f69f0-119">Parent elements</span></span>

|<span data-ttu-id="f69f0-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f69f0-120">**Element**</span></span>|<span data-ttu-id="f69f0-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="f69f0-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f69f0-122">Folder</span><span class="sxs-lookup"><span data-stu-id="f69f0-122">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="f69f0-123">Définit un dossier pour créer, obtenir, recherchez, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="f69f0-123">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="f69f0-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="f69f0-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="f69f0-125">Représente un dossier de recherche qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f69f0-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f69f0-126">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="f69f0-126">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="f69f0-127">Représente un dossier de contacts qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f69f0-127">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f69f0-128">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="f69f0-128">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="f69f0-129">Représente un dossier de tâches qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f69f0-129">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f69f0-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="f69f0-130">Remarks</span></span>

<span data-ttu-id="f69f0-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f69f0-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="f69f0-132">Cet élément a été introduit dans Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f69f0-132">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="f69f0-133">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="f69f0-133">Version differences</span></span>

<span data-ttu-id="f69f0-134">Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange commençant par Exchange 2013, les autorisations de dossier ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a une valeur de **AllProperties** dans la requête d’opération [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f69f0-134">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="f69f0-135">Pour récupérer les autorisations du dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément de [AdditionalProperties](additionalproperties.md) dans la demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="f69f0-135">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f69f0-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f69f0-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f69f0-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f69f0-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f69f0-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f69f0-138">Schema Name</span></span>  <br/> |<span data-ttu-id="f69f0-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f69f0-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="f69f0-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f69f0-140">Validation File</span></span>  <br/> |<span data-ttu-id="f69f0-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f69f0-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f69f0-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f69f0-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="f69f0-143">False</span><span class="sxs-lookup"><span data-stu-id="f69f0-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f69f0-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f69f0-144">See also</span></span>



- [<span data-ttu-id="f69f0-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f69f0-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f69f0-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="f69f0-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

