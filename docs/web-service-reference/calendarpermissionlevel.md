---
title: CalendarPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissionLevel
api_type:
- schema
ms.assetid: 6ac2b792-4326-4a3f-b6cb-977bf523b5b2
description: L’élément CalendarPermissionLevel représente le niveau d’autorisation dont dispose un utilisateur sur un dossier de calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 670f78e0b3cef7a40339c83d84916871f8969536
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527179"
---
# <a name="calendarpermissionlevel"></a><span data-ttu-id="afa0d-104">CalendarPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="afa0d-104">CalendarPermissionLevel</span></span>

<span data-ttu-id="afa0d-105">L’élément **CalendarPermissionLevel** représente le niveau d’autorisation dont dispose un utilisateur sur un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="afa0d-105">The **CalendarPermissionLevel** element represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="afa0d-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="afa0d-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or FreeBusyTimeOnly or FreeBusyTimeAndSubjectAndLocation or Custom</CalendarPermissionLevel>
```

 <span data-ttu-id="afa0d-107">**CalendarPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="afa0d-107">**CalendarPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afa0d-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="afa0d-108">Attributes and elements</span></span>

<span data-ttu-id="afa0d-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="afa0d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afa0d-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="afa0d-110">Attributes</span></span>

<span data-ttu-id="afa0d-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="afa0d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afa0d-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="afa0d-112">Child elements</span></span>

<span data-ttu-id="afa0d-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="afa0d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afa0d-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="afa0d-114">Parent elements</span></span>

|<span data-ttu-id="afa0d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="afa0d-115">**Element**</span></span>|<span data-ttu-id="afa0d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="afa0d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afa0d-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="afa0d-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="afa0d-p103">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="afa0d-p103">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afa0d-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="afa0d-120">Text value</span></span>

<span data-ttu-id="afa0d-121">Le tableau suivant répertorie les valeurs possibles pour l’élément **CalendarPermissionLevel** .</span><span class="sxs-lookup"><span data-stu-id="afa0d-121">The following table lists the possible values for the **CalendarPermissionLevel** element.</span></span> 
  
<span data-ttu-id="afa0d-122">**Valeurs de texte de l’élément CalendarPermissionLevel**</span><span class="sxs-lookup"><span data-stu-id="afa0d-122">**CalendarPermissionLevel element text values**</span></span>

|<span data-ttu-id="afa0d-123">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="afa0d-123">**Value**</span></span>|<span data-ttu-id="afa0d-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="afa0d-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="afa0d-125">Aucun</span><span class="sxs-lookup"><span data-stu-id="afa0d-125">None</span></span>  <br/> |<span data-ttu-id="afa0d-126">Indique que l’utilisateur ne dispose pas d’autorisations sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="afa0d-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="afa0d-127">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="afa0d-127">Owner</span></span>  <br/> |<span data-ttu-id="afa0d-128">Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments du dossier, et créer des sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="afa0d-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="afa0d-129">L’utilisateur est le propriétaire du dossier et le contact du dossier.</span><span class="sxs-lookup"><span data-stu-id="afa0d-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="afa0d-130">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="afa0d-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="afa0d-131">Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments du dossier, et créer des sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="afa0d-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="afa0d-132">Éditeur</span><span class="sxs-lookup"><span data-stu-id="afa0d-132">Editor</span></span>  <br/> |<span data-ttu-id="afa0d-133">Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments du dossier.</span><span class="sxs-lookup"><span data-stu-id="afa0d-133">Indicates that the user can create, read, edit and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="afa0d-134">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="afa0d-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="afa0d-135">Indique que l’utilisateur peut créer et lire tous les éléments du dossier, modifier et supprimer uniquement les éléments que l’utilisateur crée et créer des sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="afa0d-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="afa0d-136">Auteur</span><span class="sxs-lookup"><span data-stu-id="afa0d-136">Author</span></span>  <br/> |<span data-ttu-id="afa0d-137">Indique que l’utilisateur peut créer et lire tous les éléments du dossier, et modifier et supprimer uniquement les éléments créés par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="afa0d-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="afa0d-138">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="afa0d-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="afa0d-139">Indique que l’utilisateur peut créer et lire tous les éléments du dossier, et supprimer uniquement les éléments créés par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="afa0d-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="afa0d-140">Relecteur</span><span class="sxs-lookup"><span data-stu-id="afa0d-140">Reviewer</span></span>  <br/> |<span data-ttu-id="afa0d-141">Indique que l’utilisateur peut lire tous les éléments du dossier.</span><span class="sxs-lookup"><span data-stu-id="afa0d-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="afa0d-142">Collaborateur</span><span class="sxs-lookup"><span data-stu-id="afa0d-142">Contributor</span></span>  <br/> |<span data-ttu-id="afa0d-143">Indique que l’utilisateur peut créer des éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="afa0d-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="afa0d-144">Le contenu du dossier n’apparaît pas.</span><span class="sxs-lookup"><span data-stu-id="afa0d-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="afa0d-145">FreeBusyTimeOnly</span><span class="sxs-lookup"><span data-stu-id="afa0d-145">FreeBusyTimeOnly</span></span>  <br/> |<span data-ttu-id="afa0d-146">Indique que l’utilisateur peut afficher uniquement les disponibilités dans le calendrier.</span><span class="sxs-lookup"><span data-stu-id="afa0d-146">Indicates that the user can view only free/busy time within the calendar.</span></span>  <br/> |
|<span data-ttu-id="afa0d-147">FreeBusyTimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="afa0d-147">FreeBusyTimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="afa0d-148">Indique que l’utilisateur peut afficher les disponibilités dans le calendrier, l’objet et l’emplacement des rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="afa0d-148">Indicates that the user can view free/busy time within the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="afa0d-149">Personnalisé</span><span class="sxs-lookup"><span data-stu-id="afa0d-149">Custom</span></span>  <br/> |<span data-ttu-id="afa0d-150">Indique que l’utilisateur dispose d’autorisations d’accès personnalisées sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="afa0d-150">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="afa0d-151">Remarques</span><span class="sxs-lookup"><span data-stu-id="afa0d-151">Remarks</span></span>

<span data-ttu-id="afa0d-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="afa0d-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afa0d-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="afa0d-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afa0d-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="afa0d-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afa0d-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="afa0d-155">Schema Name</span></span>  <br/> |<span data-ttu-id="afa0d-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="afa0d-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="afa0d-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="afa0d-157">Validation File</span></span>  <br/> |<span data-ttu-id="afa0d-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="afa0d-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afa0d-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="afa0d-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="afa0d-160">False</span><span class="sxs-lookup"><span data-stu-id="afa0d-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afa0d-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="afa0d-161">See also</span></span>



- [<span data-ttu-id="afa0d-162">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="afa0d-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="afa0d-163">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="afa0d-163">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

