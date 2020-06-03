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
description: L’élément DelegatePermissions contient les paramètres de niveau d’autorisation délégués pour un utilisateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 2cf8c9a8d3c5db8e13d43c207df173c12fca5acb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457409"
---
# <a name="delegatepermissions"></a><span data-ttu-id="d68e7-104">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="d68e7-104">DelegatePermissions</span></span>

<span data-ttu-id="d68e7-105">L’élément **DelegatePermissions** contient les paramètres de niveau d’autorisation délégués pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d68e7-105">The **DelegatePermissions** element contains the delegate permission-level settings for a user.</span></span> <span data-ttu-id="d68e7-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d68e7-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
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

<span data-ttu-id="d68e7-107">**DelegatePermissionsType**</span><span class="sxs-lookup"><span data-stu-id="d68e7-107">**DelegatePermissionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d68e7-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d68e7-108">Attributes and elements</span></span>

<span data-ttu-id="d68e7-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d68e7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d68e7-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d68e7-110">Attributes</span></span>

<span data-ttu-id="d68e7-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d68e7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d68e7-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d68e7-112">Child elements</span></span>

|<span data-ttu-id="d68e7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d68e7-113">**Element**</span></span>|<span data-ttu-id="d68e7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d68e7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d68e7-115">CalendarFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="d68e7-115">CalendarFolderPermissionLevel</span></span>](calendarfolderpermissionlevel.md) <br/> |<span data-ttu-id="d68e7-116">Contient les autorisations pour le dossier calendrier par défaut.</span><span class="sxs-lookup"><span data-stu-id="d68e7-116">Contains the permissions for the default Calendar folder.</span></span> <span data-ttu-id="d68e7-117">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d68e7-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d68e7-118">TasksFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="d68e7-118">TasksFolderPermissionLevel</span></span>](tasksfolderpermissionlevel.md) <br/> |<span data-ttu-id="d68e7-119">Contient les autorisations pour le dossier de tâches par défaut.</span><span class="sxs-lookup"><span data-stu-id="d68e7-119">Contains the permissions for the default Task folder.</span></span> <span data-ttu-id="d68e7-120">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d68e7-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d68e7-121">InboxFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="d68e7-121">InboxFolderPermissionLevel</span></span>](inboxfolderpermissionlevel.md) <br/> |<span data-ttu-id="d68e7-122">Contient les autorisations pour le dossier boîte de réception par défaut.</span><span class="sxs-lookup"><span data-stu-id="d68e7-122">Contains the permissions for the default Inbox folder.</span></span> <span data-ttu-id="d68e7-123">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d68e7-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d68e7-124">ContactsFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="d68e7-124">ContactsFolderPermissionLevel</span></span>](contactsfolderpermissionlevel.md) <br/> |<span data-ttu-id="d68e7-125">Contient les autorisations pour le dossier de contacts par défaut.</span><span class="sxs-lookup"><span data-stu-id="d68e7-125">Contains the permissions for the default Contacts folder.</span></span> <span data-ttu-id="d68e7-126">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d68e7-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d68e7-127">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="d68e7-127">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md) <br/> |<span data-ttu-id="d68e7-128">Contient les autorisations pour le dossier Notes par défaut.</span><span class="sxs-lookup"><span data-stu-id="d68e7-128">Contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="d68e7-129">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d68e7-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d68e7-130">JournalFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="d68e7-130">JournalFolderPermissionLevel</span></span>](journalfolderpermissionlevel.md) <br/> |<span data-ttu-id="d68e7-131">Contient les autorisations pour le dossier journal par défaut.</span><span class="sxs-lookup"><span data-stu-id="d68e7-131">Contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="d68e7-132">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d68e7-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d68e7-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d68e7-133">Parent elements</span></span>

|<span data-ttu-id="d68e7-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d68e7-134">**Element**</span></span>|<span data-ttu-id="d68e7-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="d68e7-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d68e7-136">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="d68e7-136">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="d68e7-137">Identifie un seul délégué à ajouter ou mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d68e7-137">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="d68e7-138">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d68e7-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d68e7-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="d68e7-139">Remarks</span></span>

<span data-ttu-id="d68e7-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d68e7-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d68e7-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d68e7-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d68e7-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d68e7-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d68e7-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d68e7-143">Schema Name</span></span>  <br/> |<span data-ttu-id="d68e7-144">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d68e7-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="d68e7-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d68e7-145">Validation File</span></span>  <br/> |<span data-ttu-id="d68e7-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d68e7-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d68e7-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d68e7-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="d68e7-148">False</span><span class="sxs-lookup"><span data-stu-id="d68e7-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d68e7-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d68e7-149">See also</span></span>

- [<span data-ttu-id="d68e7-150">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="d68e7-150">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="d68e7-151">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="d68e7-151">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="d68e7-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d68e7-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="d68e7-153">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="d68e7-153">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

