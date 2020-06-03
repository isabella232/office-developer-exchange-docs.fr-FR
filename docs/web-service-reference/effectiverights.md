---
title: EffectiveRights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: L’élément EffectiveRights contient les droits du client en fonction des paramètres d’autorisation de l’élément ou du dossier. Cet élément est en lecture seule.
ms.openlocfilehash: 3055eb73056750508b48ead29136b56e7ce97ee9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459243"
---
# <a name="effectiverights"></a><span data-ttu-id="2ab57-104">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="2ab57-104">EffectiveRights</span></span>

<span data-ttu-id="2ab57-105">L’élément **EffectiveRights** contient les droits du client en fonction des paramètres d’autorisation de l’élément ou du dossier.</span><span class="sxs-lookup"><span data-stu-id="2ab57-105">The **EffectiveRights** element contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="2ab57-106">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="2ab57-106">This element is read-only.</span></span> 
  
```XML
<EffectiveRights>
   <CreateAssociated/>
   <CreateContents/>
   <CreateHierarchy/>
   <Delete/>
   <Modify/>
   <Read/>
   <ViewPrivateItems/>
</EffectiveRights>
```

 <span data-ttu-id="2ab57-107">**EffectiveRightsType**</span><span class="sxs-lookup"><span data-stu-id="2ab57-107">**EffectiveRightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ab57-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ab57-108">Attributes and elements</span></span>

<span data-ttu-id="2ab57-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ab57-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ab57-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ab57-110">Attributes</span></span>

<span data-ttu-id="2ab57-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2ab57-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ab57-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ab57-112">Child elements</span></span>

|<span data-ttu-id="2ab57-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ab57-113">**Element**</span></span>|<span data-ttu-id="2ab57-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ab57-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ab57-115">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="2ab57-115">CreateAssociated</span></span>](createassociated.md) <br/> |<span data-ttu-id="2ab57-116">Indique si un client peut créer une table des matières associée.</span><span class="sxs-lookup"><span data-stu-id="2ab57-116">Indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="2ab57-117">Cette propriété est utilisée uniquement sur les objets Folder.</span><span class="sxs-lookup"><span data-stu-id="2ab57-117">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-118">CreateContents</span><span class="sxs-lookup"><span data-stu-id="2ab57-118">CreateContents</span></span>](createcontents.md) <br/> |<span data-ttu-id="2ab57-119">Indique si un client peut créer une table des matières.</span><span class="sxs-lookup"><span data-stu-id="2ab57-119">Indicates whether a client can create a contents table.</span></span> <span data-ttu-id="2ab57-120">Cette propriété est utilisée uniquement sur les objets Folder.</span><span class="sxs-lookup"><span data-stu-id="2ab57-120">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-121">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="2ab57-121">CreateHierarchy</span></span>](createhierarchy.md) <br/> |<span data-ttu-id="2ab57-122">Indique si un client peut créer une table de hiérarchie.</span><span class="sxs-lookup"><span data-stu-id="2ab57-122">Indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="2ab57-123">Cette propriété est utilisée uniquement sur les objets Folder.</span><span class="sxs-lookup"><span data-stu-id="2ab57-123">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-124">Supprimer</span><span class="sxs-lookup"><span data-stu-id="2ab57-124">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="2ab57-125">Indique si un client peut supprimer un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="2ab57-125">Indicates whether a client can delete a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-126">Modify</span><span class="sxs-lookup"><span data-stu-id="2ab57-126">Modify</span></span>](modify.md) <br/> |<span data-ttu-id="2ab57-127">Indique si un client peut modifier un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="2ab57-127">Indicates whether a client can modify a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-128">Read</span><span class="sxs-lookup"><span data-stu-id="2ab57-128">Read</span></span>](read.md) <br/> |<span data-ttu-id="2ab57-129">Indique si un client peut lire un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="2ab57-129">Indicates whether a client can read a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-130">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="2ab57-130">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="2ab57-131">Indique si un élément privé peut être affiché.</span><span class="sxs-lookup"><span data-stu-id="2ab57-131">Indicates whether a private item can be viewed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2ab57-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ab57-132">Parent elements</span></span>

|<span data-ttu-id="2ab57-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ab57-133">**Element**</span></span>|<span data-ttu-id="2ab57-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ab57-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ab57-135">Folder</span><span class="sxs-lookup"><span data-stu-id="2ab57-135">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="2ab57-136">Représente un dossier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2ab57-136">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-137">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="2ab57-137">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="2ab57-138">Représente un dossier tâches dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2ab57-138">Represents a tasks folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-139">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="2ab57-139">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="2ab57-140">Représente un dossier de contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2ab57-140">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-141">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="2ab57-141">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="2ab57-142">Représente un dossier de calendrier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2ab57-142">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="2ab57-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="2ab57-144">Représente un dossier de recherche dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2ab57-144">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-145">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2ab57-145">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2ab57-146">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ab57-146">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-147">Contact</span><span class="sxs-lookup"><span data-stu-id="2ab57-147">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="2ab57-148">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ab57-148">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-149">DistributionList</span><span class="sxs-lookup"><span data-stu-id="2ab57-149">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="2ab57-150">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="2ab57-150">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-151">Élément</span><span class="sxs-lookup"><span data-stu-id="2ab57-151">Item</span></span>](item.md) <br/> |<span data-ttu-id="2ab57-152">Représente un élément Exchange générique.</span><span class="sxs-lookup"><span data-stu-id="2ab57-152">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-153">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="2ab57-153">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="2ab57-154">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ab57-154">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-155">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="2ab57-155">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="2ab57-156">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ab57-156">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-157">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="2ab57-157">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2ab57-158">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ab57-158">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-159">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="2ab57-159">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="2ab57-160">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ab57-160">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-161">Message</span><span class="sxs-lookup"><span data-stu-id="2ab57-161">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2ab57-162">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ab57-162">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-163">Tâche</span><span class="sxs-lookup"><span data-stu-id="2ab57-163">Task</span></span>](task.md) <br/> |<span data-ttu-id="2ab57-164">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ab57-164">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2ab57-165">PostItem</span><span class="sxs-lookup"><span data-stu-id="2ab57-165">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="2ab57-166">Représente un élément post dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ab57-166">Represents a post item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ab57-167">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2ab57-167">Text value</span></span>

<span data-ttu-id="2ab57-168">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ab57-168">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2ab57-169">Remarques</span><span class="sxs-lookup"><span data-stu-id="2ab57-169">Remarks</span></span>

<span data-ttu-id="2ab57-170">**EffectiveRights** est pris en charge dans les réponses GetFolder, GetItem, FindFolder, FindItem, Opérationsyncfolderhierarchy et SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="2ab57-170">**EffectiveRights** is supported in the GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy, and SyncFolderItems responses.</span></span> <span data-ttu-id="2ab57-171">La propriété **EffectiveRights** est exposée dans la forme **AllProperties** pour les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="2ab57-171">The **EffectiveRights** property is exposed in the **AllProperties** shape for folders and items.</span></span> 
  
<span data-ttu-id="2ab57-172">Cette propriété **EffectiveRights** fournit l’accès aux mêmes informations que celles fournies dans la propriété **MAPI PR_ACCESS** .</span><span class="sxs-lookup"><span data-stu-id="2ab57-172">This **EffectiveRights** property provides access to the same information that is provided in the **PR_ACCESS MAPI** property.</span></span> 
  
<span data-ttu-id="2ab57-173">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ab57-173">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ab57-174">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ab57-174">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ab57-175">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ab57-175">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ab57-176">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ab57-176">Schema Name</span></span>  <br/> |<span data-ttu-id="2ab57-177">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2ab57-177">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ab57-178">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2ab57-178">Validation File</span></span>  <br/> |<span data-ttu-id="2ab57-179">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2ab57-179">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ab57-180">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ab57-180">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ab57-181">False</span><span class="sxs-lookup"><span data-stu-id="2ab57-181">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ab57-182">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2ab57-182">See also</span></span>

- [<span data-ttu-id="2ab57-183">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2ab57-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="2ab57-184">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="2ab57-184">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

