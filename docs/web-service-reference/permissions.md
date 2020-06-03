---
title: Autorisations
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permissions
api_type:
- schema
ms.assetid: 2ba50bd9-819f-4e5f-a3bb-85a0a87d8a86
description: L’élément permissions contient la collection d’autorisations pour un dossier.
ms.openlocfilehash: b8616cefdb8c453106753fb0788a6c7d6a0ded79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459215"
---
# <a name="permissions"></a><span data-ttu-id="74428-103">Autorisations</span><span class="sxs-lookup"><span data-stu-id="74428-103">Permissions</span></span>

<span data-ttu-id="74428-104">L’élément **permissions** contient la collection d’autorisations pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="74428-104">The **Permissions** element contains the collection of permissions for a folder.</span></span> 
  
```XML
<Permissions>
   <Permission/>
</Permissions>
```

 <span data-ttu-id="74428-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="74428-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74428-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="74428-106">Attributes and elements</span></span>

<span data-ttu-id="74428-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="74428-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74428-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="74428-108">Attributes</span></span>

<span data-ttu-id="74428-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="74428-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74428-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="74428-110">Child elements</span></span>

|<span data-ttu-id="74428-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="74428-111">**Element**</span></span>|<span data-ttu-id="74428-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="74428-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74428-113">Autorisation</span><span class="sxs-lookup"><span data-stu-id="74428-113">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="74428-114">Définit l’accès d’un délégué à un dossier.</span><span class="sxs-lookup"><span data-stu-id="74428-114">Defines the access that a delegate has to a folder.</span></span> <span data-ttu-id="74428-115">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="74428-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74428-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="74428-116">Parent elements</span></span>

|<span data-ttu-id="74428-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="74428-117">**Element**</span></span>|<span data-ttu-id="74428-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="74428-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74428-119">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="74428-119">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="74428-120">Contient toutes les autorisations configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="74428-120">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="74428-121">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="74428-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="74428-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="74428-122">Remarks</span></span>

<span data-ttu-id="74428-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="74428-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="74428-124">Cet élément a été introduit dans Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="74428-124">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="74428-125">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="74428-125">Version differences</span></span>

<span data-ttu-id="74428-126">Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange à partir d’Exchange 2013, les autorisations de dossiers ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a une valeur de **AllProperties** dans la demande d’opération [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="74428-126">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="74428-127">Pour récupérer les autorisations de dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément [AdditionalProperties](additionalproperties.md) dans la demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="74428-127">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="74428-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="74428-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74428-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="74428-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="74428-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="74428-130">Schema Name</span></span>  <br/> |<span data-ttu-id="74428-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="74428-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="74428-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="74428-132">Validation File</span></span>  <br/> |<span data-ttu-id="74428-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="74428-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="74428-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="74428-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="74428-135">False</span><span class="sxs-lookup"><span data-stu-id="74428-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74428-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="74428-136">See also</span></span>



- [<span data-ttu-id="74428-137">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="74428-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="74428-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="74428-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

