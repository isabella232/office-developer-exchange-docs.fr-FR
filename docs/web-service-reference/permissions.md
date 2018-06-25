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
description: L’élément Permissions contient la collection des autorisations pour un dossier.
ms.openlocfilehash: 08d015c3b1afb58fce0fb4b99466965cc5c29fc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828727"
---
# <a name="permissions"></a><span data-ttu-id="683ea-103">Autorisations</span><span class="sxs-lookup"><span data-stu-id="683ea-103">Permissions</span></span>

<span data-ttu-id="683ea-104">L’élément **Permissions** contient la collection des autorisations pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="683ea-104">The **Permissions** element contains the collection of permissions for a folder.</span></span> 
  
```XML
<Permissions>
   <Permission/>
</Permissions>
```

 <span data-ttu-id="683ea-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="683ea-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="683ea-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="683ea-106">Attributes and elements</span></span>

<span data-ttu-id="683ea-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="683ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="683ea-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="683ea-108">Attributes</span></span>

<span data-ttu-id="683ea-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="683ea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="683ea-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="683ea-110">Child elements</span></span>

|<span data-ttu-id="683ea-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="683ea-111">**Element**</span></span>|<span data-ttu-id="683ea-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="683ea-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="683ea-113">Autorisation</span><span class="sxs-lookup"><span data-stu-id="683ea-113">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="683ea-114">Définit l’accès délégué à un dossier.</span><span class="sxs-lookup"><span data-stu-id="683ea-114">Defines the access that a delegate has to a folder.</span></span> <span data-ttu-id="683ea-115">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="683ea-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="683ea-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="683ea-116">Parent elements</span></span>

|<span data-ttu-id="683ea-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="683ea-117">**Element**</span></span>|<span data-ttu-id="683ea-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="683ea-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="683ea-119">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="683ea-119">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="683ea-120">Contient toutes les autorisations qui sont configurées pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="683ea-120">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="683ea-121">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="683ea-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="683ea-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="683ea-122">Remarks</span></span>

<span data-ttu-id="683ea-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="683ea-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="683ea-124">Cet élément a été introduit dans Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="683ea-124">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="683ea-125">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="683ea-125">Version differences</span></span>

<span data-ttu-id="683ea-126">Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange commençant par Exchange 2013, les autorisations de dossier ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a une valeur de **AllProperties** dans la requête d’opération [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="683ea-126">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="683ea-127">Pour récupérer les autorisations du dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément de [AdditionalProperties](additionalproperties.md) dans la demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="683ea-127">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="683ea-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="683ea-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="683ea-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="683ea-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="683ea-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="683ea-130">Schema Name</span></span>  <br/> |<span data-ttu-id="683ea-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="683ea-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="683ea-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="683ea-132">Validation File</span></span>  <br/> |<span data-ttu-id="683ea-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="683ea-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="683ea-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="683ea-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="683ea-135">False</span><span class="sxs-lookup"><span data-stu-id="683ea-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="683ea-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="683ea-136">See also</span></span>



- [<span data-ttu-id="683ea-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="683ea-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="683ea-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="683ea-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

