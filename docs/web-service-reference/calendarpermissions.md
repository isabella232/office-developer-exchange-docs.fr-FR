---
title: CalendarPermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissions
api_type:
- schema
ms.assetid: 9b659d83-45fb-42a2-b052-5bc4dbe3854d
description: L’élément CalendarPermissions contient un tableau d’autorisations pour un dossier de calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 3dee635e4449cbb3717f5d2fab8838f3e43102a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755479"
---
# <a name="calendarpermissions"></a><span data-ttu-id="18b59-104">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="18b59-104">CalendarPermissions</span></span>

<span data-ttu-id="18b59-105">L’élément **CalendarPermissions** contient un tableau d’autorisations pour un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="18b59-105">The **CalendarPermissions** element contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="18b59-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="18b59-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissions>
   <PermissionSet/>
</CalendarPermissions>
```

 <span data-ttu-id="18b59-107">**ArrayOfCalendarPermissionsType**</span><span class="sxs-lookup"><span data-stu-id="18b59-107">**ArrayOfCalendarPermissionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18b59-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="18b59-108">Attributes and elements</span></span>

<span data-ttu-id="18b59-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="18b59-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18b59-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="18b59-110">Attributes</span></span>

<span data-ttu-id="18b59-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="18b59-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18b59-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="18b59-112">Child elements</span></span>

|<span data-ttu-id="18b59-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="18b59-113">**Element**</span></span>|<span data-ttu-id="18b59-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="18b59-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18b59-115">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="18b59-115">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="18b59-116">Définit l’accès dont dispose un utilisateur délégué à un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="18b59-116">Defines the access that a delegate user has to a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18b59-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="18b59-117">Parent elements</span></span>

|<span data-ttu-id="18b59-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="18b59-118">**Element**</span></span>|<span data-ttu-id="18b59-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="18b59-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18b59-120">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="18b59-120">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="18b59-121">Contient toutes les autorisations configurées pour un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="18b59-121">Contains all the configured permissions for a calendar folder.</span></span> <span data-ttu-id="18b59-122">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="18b59-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="18b59-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="18b59-123">Remarks</span></span>

<span data-ttu-id="18b59-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="18b59-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18b59-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="18b59-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18b59-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="18b59-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18b59-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="18b59-127">Schema Name</span></span>  <br/> |<span data-ttu-id="18b59-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="18b59-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="18b59-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="18b59-129">Validation File</span></span>  <br/> |<span data-ttu-id="18b59-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="18b59-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18b59-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="18b59-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="18b59-132">False</span><span class="sxs-lookup"><span data-stu-id="18b59-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18b59-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="18b59-133">See also</span></span>



- [<span data-ttu-id="18b59-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="18b59-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="18b59-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="18b59-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

