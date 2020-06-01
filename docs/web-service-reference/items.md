---
title: Éléments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: 0811a73e-bf1f-4889-9219-73902dd47639
description: L’élément ITEMS contient un tableau d’éléments.
ms.openlocfilehash: 489e34ad0e4bcc2520febb3c213db970fa496051
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458130"
---
# <a name="items"></a><span data-ttu-id="400b8-103">Éléments</span><span class="sxs-lookup"><span data-stu-id="400b8-103">Items</span></span>

<span data-ttu-id="400b8-104">L’élément **Items** contient un tableau d’éléments.</span><span class="sxs-lookup"><span data-stu-id="400b8-104">The **Items** element contains an array of items.</span></span> 
  
```xml
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <PostItem/>
</Items>
```

 <span data-ttu-id="400b8-105">**ArrayOfRealItemsType**</span><span class="sxs-lookup"><span data-stu-id="400b8-105">**ArrayOfRealItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="400b8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="400b8-106">Attributes and elements</span></span>

<span data-ttu-id="400b8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="400b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="400b8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="400b8-108">Attributes</span></span>

<span data-ttu-id="400b8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="400b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="400b8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="400b8-110">Child elements</span></span>

|<span data-ttu-id="400b8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="400b8-111">**Element**</span></span>|<span data-ttu-id="400b8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="400b8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="400b8-113">Élément</span><span class="sxs-lookup"><span data-stu-id="400b8-113">Item</span></span>](item.md) <br/> |<span data-ttu-id="400b8-114">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="400b8-114">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="400b8-115">Message</span><span class="sxs-lookup"><span data-stu-id="400b8-115">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="400b8-116">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="400b8-116">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="400b8-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="400b8-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="400b8-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="400b8-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="400b8-119">Contact</span><span class="sxs-lookup"><span data-stu-id="400b8-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="400b8-120">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="400b8-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="400b8-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="400b8-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="400b8-122">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="400b8-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="400b8-123">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="400b8-123">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="400b8-124">Représente un message de réunion dans la Banque d’aide Exchange.</span><span class="sxs-lookup"><span data-stu-id="400b8-124">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="400b8-125">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="400b8-125">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="400b8-126">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="400b8-126">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="400b8-127">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="400b8-127">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="400b8-128">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="400b8-128">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="400b8-129">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="400b8-129">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="400b8-130">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="400b8-130">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="400b8-131">Tâche</span><span class="sxs-lookup"><span data-stu-id="400b8-131">Task</span></span>](task.md) <br/> |<span data-ttu-id="400b8-132">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="400b8-132">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="400b8-133">PostItem</span><span class="sxs-lookup"><span data-stu-id="400b8-133">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="400b8-134">Représente un élément post dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="400b8-134">Represents a post item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="400b8-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="400b8-135">Parent elements</span></span>

|<span data-ttu-id="400b8-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="400b8-136">**Element**</span></span>|<span data-ttu-id="400b8-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="400b8-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="400b8-138">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="400b8-138">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md) <br/> |<span data-ttu-id="400b8-139">Contient l’État et le résultat d’une demande d' [opération CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="400b8-139">Contains the status and result of a [CopyItem operation](copyitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="400b8-140">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="400b8-140">CreateItemResponseMessage</span></span>](createitemresponsemessage.md) <br/> |<span data-ttu-id="400b8-141">Contient l’État et le résultat d’une seule demande d' [opération CreateItem](createitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="400b8-141">Contains the status and result of a single [CreateItem operation](createitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="400b8-142">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="400b8-142">GetItemResponseMessage</span></span>](getitemresponsemessage.md) <br/> |<span data-ttu-id="400b8-143">Contient l’État et le résultat d’une demande d' [opération GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="400b8-143">Contains the status and result of a [GetItem operation](getitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="400b8-144">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="400b8-144">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="400b8-145">Représente une collection d’éléments qui sont le résultat d’un appel d' [opération FindItem](finditem-operation.md) groupé.</span><span class="sxs-lookup"><span data-stu-id="400b8-145">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="400b8-146">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="400b8-146">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md) <br/> |<span data-ttu-id="400b8-147">Contient l’État et le résultat d’une demande d' [opération MoveItem](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="400b8-147">Contains the status and result of a [MoveItem operation](moveitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="400b8-148">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="400b8-148">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="400b8-149">Contient les résultats d’une recherche d’un dossier racine unique pendant une [opération FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="400b8-149">Contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="400b8-150">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="400b8-150">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="400b8-151">Contient l’État et le résultat d’une demande d' [opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="400b8-151">Contains the status and result of an [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="400b8-152">Remarques</span><span class="sxs-lookup"><span data-stu-id="400b8-152">Remarks</span></span>

<span data-ttu-id="400b8-153">Pour plus d’informations sur l’ensemble d’éléments d’une demande de [commande CreateItem](createitem-operation.md) , voir [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md).</span><span class="sxs-lookup"><span data-stu-id="400b8-153">For information about the set of items in a [CreateItem operation](createitem-operation.md) request, see [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md).</span></span>
  
<span data-ttu-id="400b8-154">Les éléments de [message](message-ex15websvcsotherref.md) représentent les messages électroniques et tous les autres éléments qui ne sont pas fortement typés par le schéma des services Web Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="400b8-154">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="400b8-155">Des éléments tels que IPM. Le partage et IPM. InfoPath sont renvoyés en tant qu’éléments **message** .</span><span class="sxs-lookup"><span data-stu-id="400b8-155">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="400b8-156">Les versions d’Exchange commençant par Exchange Server 2010 ne renvoient pas l’élément [élément](item.md) de base dans les réponses.</span><span class="sxs-lookup"><span data-stu-id="400b8-156">Versions of Exchange starting with Exchange Server 2010 do not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="400b8-157">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="400b8-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="400b8-158">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="400b8-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="400b8-159">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="400b8-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="400b8-160">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="400b8-160">Schema Name</span></span>  <br/> |<span data-ttu-id="400b8-161">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="400b8-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="400b8-162">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="400b8-162">Validation File</span></span>  <br/> |<span data-ttu-id="400b8-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="400b8-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="400b8-164">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="400b8-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="400b8-165">False</span><span class="sxs-lookup"><span data-stu-id="400b8-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="400b8-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="400b8-166">See also</span></span>



[<span data-ttu-id="400b8-167">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="400b8-167">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
  
- [<span data-ttu-id="400b8-168">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="400b8-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

