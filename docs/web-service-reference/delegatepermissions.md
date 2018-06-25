---
title: DelegatePermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegatePermissions
api_type:
- schema
ms.assetid: 292badc7-bab3-4368-9d7c-9a8b7edb279b
description: L’élément DelegatePermissions contient les paramètres de niveau d’autorisation de délégué pour un utilisateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 319592b6c3386a07b3094115c335c7fb8ffe1130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755834"
---
# <a name="delegatepermissions"></a><span data-ttu-id="1cbdb-104">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="1cbdb-104">DelegatePermissions</span></span>

<span data-ttu-id="1cbdb-105">L’élément **DelegatePermissions** contient les paramètres de niveau d’autorisation de délégué pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-105">The **DelegatePermissions** element contains the delegate permission-level settings for a user.</span></span> <span data-ttu-id="1cbdb-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1cbdb-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegatePermissions>
   <CalendarFolderPermissionLevel/>
   <TasksFolderPermissionLevel/>
   <InboxFolderPermissionLevel/>
   <ContactsFolderPermissionLevel/>
   <NotesFolderPermissionLevel/>
   <JournalFolderPermissionLevel/>
</DelegatePermissions>
```

<span data-ttu-id="1cbdb-107">**DelegatePermissionsType**</span><span class="sxs-lookup"><span data-stu-id="1cbdb-107">**DelegatePermissionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1cbdb-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1cbdb-108">Attributes and elements</span></span>

<span data-ttu-id="1cbdb-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cbdb-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="1cbdb-110">Attributes</span></span>

<span data-ttu-id="1cbdb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cbdb-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1cbdb-112">Child elements</span></span>

|<span data-ttu-id="1cbdb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1cbdb-113">**Element**</span></span>|<span data-ttu-id="1cbdb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1cbdb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cbdb-115">CalendarFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="1cbdb-115">CalendarFolderPermissionLevel</span></span>](calendarfolderpermissionlevel.md) <br/> |<span data-ttu-id="1cbdb-116">Contient les autorisations pour le dossier calendrier par défaut.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-116">Contains the permissions for the default Calendar folder.</span></span> <span data-ttu-id="1cbdb-117">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="1cbdb-118">TasksFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="1cbdb-118">TasksFolderPermissionLevel</span></span>](tasksfolderpermissionlevel.md) <br/> |<span data-ttu-id="1cbdb-119">Contient les autorisations pour le dossier tâches par défaut.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-119">Contains the permissions for the default Task folder.</span></span> <span data-ttu-id="1cbdb-120">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="1cbdb-121">InboxFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="1cbdb-121">InboxFolderPermissionLevel</span></span>](inboxfolderpermissionlevel.md) <br/> |<span data-ttu-id="1cbdb-122">Contient les autorisations pour le dossier boîte de réception par défaut.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-122">Contains the permissions for the default Inbox folder.</span></span> <span data-ttu-id="1cbdb-123">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="1cbdb-124">ContactsFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="1cbdb-124">ContactsFolderPermissionLevel</span></span>](contactsfolderpermissionlevel.md) <br/> |<span data-ttu-id="1cbdb-125">Contient les autorisations pour le dossier Contacts par défaut.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-125">Contains the permissions for the default Contacts folder.</span></span> <span data-ttu-id="1cbdb-126">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="1cbdb-127">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="1cbdb-127">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md) <br/> |<span data-ttu-id="1cbdb-128">Contient les autorisations pour le dossier Notes par défaut.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-128">Contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="1cbdb-129">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="1cbdb-130">JournalFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="1cbdb-130">JournalFolderPermissionLevel</span></span>](journalfolderpermissionlevel.md) <br/> |<span data-ttu-id="1cbdb-131">Contient les autorisations pour le dossier de Journal par défaut.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-131">Contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="1cbdb-132">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1cbdb-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1cbdb-133">Parent elements</span></span>

|<span data-ttu-id="1cbdb-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1cbdb-134">**Element**</span></span>|<span data-ttu-id="1cbdb-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="1cbdb-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cbdb-136">Utilisateur_délégué</span><span class="sxs-lookup"><span data-stu-id="1cbdb-136">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="1cbdb-137">Identifie un délégué pour ajouter ou mettre à jour dans une boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-137">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="1cbdb-138">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1cbdb-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="1cbdb-139">Remarks</span></span>

<span data-ttu-id="1cbdb-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1cbdb-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cbdb-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1cbdb-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cbdb-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1cbdb-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1cbdb-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1cbdb-143">Schema Name</span></span>  <br/> |<span data-ttu-id="1cbdb-144">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1cbdb-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="1cbdb-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1cbdb-145">Validation File</span></span>  <br/> |<span data-ttu-id="1cbdb-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1cbdb-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1cbdb-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1cbdb-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cbdb-148">False</span><span class="sxs-lookup"><span data-stu-id="1cbdb-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cbdb-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1cbdb-149">See also</span></span>

- [<span data-ttu-id="1cbdb-150">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="1cbdb-150">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="1cbdb-151">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="1cbdb-151">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="1cbdb-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1cbdb-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="1cbdb-153">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="1cbdb-153">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

