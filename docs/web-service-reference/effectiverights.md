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
description: L’élément EffectiveRights contient des droits du client en fonction des paramètres d’autorisation pour l’élément ou le dossier. Cet élément est en lecture seule.
ms.openlocfilehash: 610d9e214a8de648ece667799bb5e67dfcc358f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756088"
---
# <a name="effectiverights"></a><span data-ttu-id="cf981-104">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="cf981-104">EffectiveRights</span></span>

<span data-ttu-id="cf981-105">L’élément **EffectiveRights** contient des droits du client en fonction des paramètres d’autorisation pour l’élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="cf981-105">The **EffectiveRights** element contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="cf981-106">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="cf981-106">This element is read-only.</span></span> 
  
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

 <span data-ttu-id="cf981-107">**EffectiveRightsType**</span><span class="sxs-lookup"><span data-stu-id="cf981-107">**EffectiveRightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf981-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cf981-108">Attributes and elements</span></span>

<span data-ttu-id="cf981-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cf981-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf981-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="cf981-110">Attributes</span></span>

<span data-ttu-id="cf981-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cf981-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf981-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cf981-112">Child elements</span></span>

|<span data-ttu-id="cf981-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf981-113">**Element**</span></span>|<span data-ttu-id="cf981-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf981-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf981-115">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="cf981-115">CreateAssociated</span></span>](createassociated.md) <br/> |<span data-ttu-id="cf981-116">Indique si un client peut créer une table de contenu associée.</span><span class="sxs-lookup"><span data-stu-id="cf981-116">Indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="cf981-117">Cette propriété est utilisée uniquement avec des objets folder.</span><span class="sxs-lookup"><span data-stu-id="cf981-117">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="cf981-118">CreateContents</span><span class="sxs-lookup"><span data-stu-id="cf981-118">CreateContents</span></span>](createcontents.md) <br/> |<span data-ttu-id="cf981-119">Indique si un client peut créer une table des matières.</span><span class="sxs-lookup"><span data-stu-id="cf981-119">Indicates whether a client can create a contents table.</span></span> <span data-ttu-id="cf981-120">Cette propriété est utilisée uniquement avec des objets folder.</span><span class="sxs-lookup"><span data-stu-id="cf981-120">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="cf981-121">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="cf981-121">CreateHierarchy</span></span>](createhierarchy.md) <br/> |<span data-ttu-id="cf981-122">Indique si un client peut créer une table de hiérarchie.</span><span class="sxs-lookup"><span data-stu-id="cf981-122">Indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="cf981-123">Cette propriété est utilisée uniquement avec des objets folder.</span><span class="sxs-lookup"><span data-stu-id="cf981-123">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="cf981-124">Supprimer</span><span class="sxs-lookup"><span data-stu-id="cf981-124">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="cf981-125">Indique si un client peut supprimer un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="cf981-125">Indicates whether a client can delete a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="cf981-126">Modifier</span><span class="sxs-lookup"><span data-stu-id="cf981-126">Modify</span></span>](modify.md) <br/> |<span data-ttu-id="cf981-127">Indique si un client peut modifier un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="cf981-127">Indicates whether a client can modify a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="cf981-128">Read</span><span class="sxs-lookup"><span data-stu-id="cf981-128">Read</span></span>](read.md) <br/> |<span data-ttu-id="cf981-129">Indique si un client peut lire un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="cf981-129">Indicates whether a client can read a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="cf981-130">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="cf981-130">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="cf981-131">Indique si un élément privé peut être affiché.</span><span class="sxs-lookup"><span data-stu-id="cf981-131">Indicates whether a private item can be viewed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf981-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cf981-132">Parent elements</span></span>

|<span data-ttu-id="cf981-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf981-133">**Element**</span></span>|<span data-ttu-id="cf981-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf981-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf981-135">Folder</span><span class="sxs-lookup"><span data-stu-id="cf981-135">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="cf981-136">Représente un dossier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cf981-136">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cf981-137">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="cf981-137">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="cf981-138">Représente un dossier de tâches dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cf981-138">Represents a tasks folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cf981-139">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="cf981-139">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="cf981-140">Représente un dossier contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cf981-140">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cf981-141">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="cf981-141">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="cf981-142">Représente un dossier de calendrier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cf981-142">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cf981-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="cf981-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="cf981-144">Représente un dossier de recherche dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cf981-144">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cf981-145">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="cf981-145">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="cf981-146">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf981-146">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="cf981-147">Contact</span><span class="sxs-lookup"><span data-stu-id="cf981-147">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="cf981-148">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf981-148">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="cf981-149">DistributionList</span><span class="sxs-lookup"><span data-stu-id="cf981-149">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="cf981-150">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="cf981-150">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="cf981-151">Item</span><span class="sxs-lookup"><span data-stu-id="cf981-151">Item</span></span>](item.md) <br/> |<span data-ttu-id="cf981-152">Représente un élément Exchange générique.</span><span class="sxs-lookup"><span data-stu-id="cf981-152">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="cf981-153">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="cf981-153">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="cf981-154">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf981-154">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cf981-155">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="cf981-155">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="cf981-156">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf981-156">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cf981-157">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="cf981-157">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="cf981-158">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf981-158">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cf981-159">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="cf981-159">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="cf981-160">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf981-160">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cf981-161">Message</span><span class="sxs-lookup"><span data-stu-id="cf981-161">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="cf981-162">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf981-162">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="cf981-163">Tâche</span><span class="sxs-lookup"><span data-stu-id="cf981-163">Task</span></span>](task.md) <br/> |<span data-ttu-id="cf981-164">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf981-164">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cf981-165">Objet postItem</span><span class="sxs-lookup"><span data-stu-id="cf981-165">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="cf981-166">Représente un élément de publication dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf981-166">Represents a post item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf981-167">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cf981-167">Text value</span></span>

<span data-ttu-id="cf981-168">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cf981-168">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cf981-169">Remarques</span><span class="sxs-lookup"><span data-stu-id="cf981-169">Remarks</span></span>

<span data-ttu-id="cf981-170">**EffectiveRights** est pris en charge dans les réponses GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy et SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="cf981-170">**EffectiveRights** is supported in the GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy, and SyncFolderItems responses.</span></span> <span data-ttu-id="cf981-171">La propriété **EffectiveRights** est exposée dans la forme **AllProperties** des dossiers et des éléments.</span><span class="sxs-lookup"><span data-stu-id="cf981-171">The **EffectiveRights** property is exposed in the **AllProperties** shape for folders and items.</span></span> 
  
<span data-ttu-id="cf981-172">Cette propriété **EffectiveRights** permet d’accéder aux mêmes informations qui sont fournies dans la propriété **PR_ACCESS MAPI** .</span><span class="sxs-lookup"><span data-stu-id="cf981-172">This **EffectiveRights** property provides access to the same information that is provided in the **PR_ACCESS MAPI** property.</span></span> 
  
<span data-ttu-id="cf981-173">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf981-173">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf981-174">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cf981-174">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf981-175">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cf981-175">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf981-176">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cf981-176">Schema Name</span></span>  <br/> |<span data-ttu-id="cf981-177">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cf981-177">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf981-178">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cf981-178">Validation File</span></span>  <br/> |<span data-ttu-id="cf981-179">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cf981-179">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf981-180">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cf981-180">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf981-181">False</span><span class="sxs-lookup"><span data-stu-id="cf981-181">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf981-182">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cf981-182">See also</span></span>

- [<span data-ttu-id="cf981-183">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cf981-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="cf981-184">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="cf981-184">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

