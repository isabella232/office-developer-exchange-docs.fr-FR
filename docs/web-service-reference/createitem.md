---
title: CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: L’élément CreateItem définit une demande pour créer un élément dans la banque d’informations Exchange.
ms.openlocfilehash: bb5cddd5ea4fa1b73c424275a0b0219ce3e189e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755724"
---
# <a name="createitem"></a><span data-ttu-id="a0c77-103">CreateItem</span><span class="sxs-lookup"><span data-stu-id="a0c77-103">CreateItem</span></span>

<span data-ttu-id="a0c77-104">L’élément **CreateItem** définit une demande pour créer un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0c77-104">The **CreateItem** element defines a request to create an item in the Exchange store.</span></span> 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

 <span data-ttu-id="a0c77-105">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="a0c77-105">**CreateItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0c77-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a0c77-106">Attributes and elements</span></span>

<span data-ttu-id="a0c77-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a0c77-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0c77-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a0c77-108">Attributes</span></span>

|<span data-ttu-id="a0c77-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a0c77-109">**Attribute**</span></span>|<span data-ttu-id="a0c77-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0c77-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0c77-111">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="a0c77-111">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="a0c77-112">Décrit comment l’élément est traité après sa création.</span><span class="sxs-lookup"><span data-stu-id="a0c77-112">Describes how the item will be handled after it is created.</span></span> <span data-ttu-id="a0c77-113">L’attribut est requis pour les messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="a0c77-113">The attribute is required for e-mail messages.</span></span> <span data-ttu-id="a0c77-114">Cet attribut est uniquement applicable aux messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="a0c77-114">This attribute is only applicable to e-mail messages.</span></span>  <br/> |
|<span data-ttu-id="a0c77-115">**SendMeetingInvitations**</span><span class="sxs-lookup"><span data-stu-id="a0c77-115">**SendMeetingInvitations**</span></span> <br/> |<span data-ttu-id="a0c77-116">Décrit comment les demandes de réunion sont gérés après leur création.</span><span class="sxs-lookup"><span data-stu-id="a0c77-116">Describes how meeting requests are handled after they are created.</span></span> <span data-ttu-id="a0c77-117">Cet attribut est requis pour les éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="a0c77-117">This attribute is required for calendar items.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="a0c77-118">Attribut MessageDisposition</span><span class="sxs-lookup"><span data-stu-id="a0c77-118">MessageDisposition Attribute</span></span>

|<span data-ttu-id="a0c77-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a0c77-119">**Value**</span></span>|<span data-ttu-id="a0c77-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0c77-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0c77-121">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="a0c77-121">SaveOnly</span></span>  <br/> |<span data-ttu-id="a0c77-122">L’élément de message est enregistré dans le dossier spécifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="a0c77-122">The message item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="a0c77-123">Messages peuvent être envoyés ultérieurement à l’aide de l' [opération SendItem](senditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a0c77-123">Messages can be sent later by using the [SendItem operation](senditem-operation.md).</span></span> <span data-ttu-id="a0c77-124">Un identificateur d’élément est retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="a0c77-124">An item identifier is returned in the response.</span></span> <span data-ttu-id="a0c77-125">Identificateurs d’éléments ne sont pas renvoyées pour les types d’éléments à l’exception des éléments de message.</span><span class="sxs-lookup"><span data-stu-id="a0c77-125">Item identifiers are not returned for any item types except for message items.</span></span> <span data-ttu-id="a0c77-126">Cela inclut des objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="a0c77-126">This includes response objects.</span></span>  <br/> |
|<span data-ttu-id="a0c77-127">SendOnly</span><span class="sxs-lookup"><span data-stu-id="a0c77-127">SendOnly</span></span>  <br/> |<span data-ttu-id="a0c77-128">L’élément est envoyé, mais aucune copie n’est enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="a0c77-128">The item is sent but no copy is saved in the Sent Items folder.</span></span> <span data-ttu-id="a0c77-129">Un identificateur d’élément n’est pas retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="a0c77-129">An item identifier is not returned in the response.</span></span>  <br/> <span data-ttu-id="a0c77-130">> [!NOTE]> **CreateItem** ne prend pas en charge les accès délégué lorsque l’option SendOnly est utilisée, car un dossier de destination ne peut pas être spécifié avec cette option.</span><span class="sxs-lookup"><span data-stu-id="a0c77-130">> [!NOTE]> **CreateItem** does not support delegate access when the SendOnly option is used because a destination folder cannot be specified with this option.</span></span> <span data-ttu-id="a0c77-131">La solution de contournement consiste à créer l’élément, obtenir l’identificateur d’élément et ensuite utiliser l’opération SendItem pour envoyer l’élément.</span><span class="sxs-lookup"><span data-stu-id="a0c77-131">The workaround is to create the item, get the item identifier, and then use the SendItem operation to send the item.</span></span>           |
|<span data-ttu-id="a0c77-132">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="a0c77-132">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="a0c77-133">L’élément est envoyé et une copie est enregistrée dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="a0c77-133">The item is sent and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="a0c77-134">Un identificateur d’élément n’est pas retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="a0c77-134">An item identifier is not returned in the response.</span></span>  <br/> <span data-ttu-id="a0c77-135">> [!NOTE]> Demandes de réunion ne sont pas enregistrées dans le dossier identifié par la propriété [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="a0c77-135">> [!NOTE]> Meeting requests are not saved to the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) property.</span></span> <span data-ttu-id="a0c77-136">Du calendrier, uniquement l’enregistrement emplacement des éléments de calendrier peut être spécifié par la propriété **SavedItemFolderId** .</span><span class="sxs-lookup"><span data-stu-id="a0c77-136">For calendaring, only the save location for calendar items can be specified by the **SavedItemFolderId** property.</span></span> <span data-ttu-id="a0c77-137">Vous ne pouvez pas contrôler où une demande de réunion élément est enregistrée.</span><span class="sxs-lookup"><span data-stu-id="a0c77-137">You cannot control where a meeting request item is saved.</span></span> <span data-ttu-id="a0c77-138">Seuls les éléments associés sont copiés et enregistrés dans le dossier identifié par la propriété **SavedItemFolderId** .</span><span class="sxs-lookup"><span data-stu-id="a0c77-138">Only the associated calendar items are copied and saved into the folder that is identified by the **SavedItemFolderId** property.</span></span>           |
   
#### <a name="sendmeetinginvitations-attribute"></a><span data-ttu-id="a0c77-139">Attribut SendMeetingInvitations</span><span class="sxs-lookup"><span data-stu-id="a0c77-139">SendMeetingInvitations Attribute</span></span>

|<span data-ttu-id="a0c77-140">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a0c77-140">**Value**</span></span>|<span data-ttu-id="a0c77-141">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0c77-141">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0c77-142">SendToNone</span><span class="sxs-lookup"><span data-stu-id="a0c77-142">SendToNone</span></span>  <br/> |<span data-ttu-id="a0c77-143">Si l’élément est une demande de réunion, il est enregistré sous la forme d’un élément de calendrier, mais pas envoyé.</span><span class="sxs-lookup"><span data-stu-id="a0c77-143">If the item is a meeting request, it is saved as a calendar item but not sent.</span></span>  <br/> |
|<span data-ttu-id="a0c77-144">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="a0c77-144">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="a0c77-145">La demande de réunion est envoyée à tous les participants, mais n’est pas enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="a0c77-145">The meeting request is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="a0c77-146">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="a0c77-146">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="a0c77-147">La demande de réunion est envoyée à tous les participants et une copie est enregistrée dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="a0c77-147">The meeting request is sent to all attendees and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a0c77-148">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a0c77-148">Child elements</span></span>

|<span data-ttu-id="a0c77-149">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0c77-149">**Element**</span></span>|<span data-ttu-id="a0c77-150">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0c77-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0c77-151">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="a0c77-151">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="a0c77-152">Identifie le dossier cible où un nouvel élément peut être créé.</span><span class="sxs-lookup"><span data-stu-id="a0c77-152">Identifies the target folder where a new item can be created.</span></span> <span data-ttu-id="a0c77-153">Si l’attribut **MessageDisposition** est défini à SendOnly, un message créé est uniquement envoyé.</span><span class="sxs-lookup"><span data-stu-id="a0c77-153">If the **MessageDisposition** attribute is set to SendOnly, a created message will only be sent.</span></span> <span data-ttu-id="a0c77-154">Le message n’est pas placé dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="a0c77-154">The message will not be put in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="a0c77-155">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="a0c77-155">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="a0c77-156">Contient un tableau d’éléments à créer dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="a0c77-156">Contains an array of items to create in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a0c77-157">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a0c77-157">Parent elements</span></span>

<span data-ttu-id="a0c77-158">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a0c77-158">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a0c77-159">Remarques</span><span class="sxs-lookup"><span data-stu-id="a0c77-159">Remarks</span></span>

<span data-ttu-id="a0c77-160">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a0c77-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0c77-161">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a0c77-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0c77-162">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a0c77-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a0c77-163">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a0c77-163">Schema Name</span></span>  <br/> |<span data-ttu-id="a0c77-164">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a0c77-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a0c77-165">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a0c77-165">Validation File</span></span>  <br/> |<span data-ttu-id="a0c77-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a0c77-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0c77-167">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a0c77-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0c77-168">False</span><span class="sxs-lookup"><span data-stu-id="a0c77-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0c77-169">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a0c77-169">See also</span></span>



[<span data-ttu-id="a0c77-170">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="a0c77-170">CreateItemResponse</span></span>](createitemresponse.md)
  
[<span data-ttu-id="a0c77-171">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="a0c77-171">CreateItem operation</span></span>](createitem-operation.md)
  
 <span data-ttu-id="a0c77-172">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="a0c77-172">**CreateItemType**</span></span>


[<span data-ttu-id="a0c77-173">Création de Messages électroniques</span><span class="sxs-lookup"><span data-stu-id="a0c77-173">Creating E-mail Messages</span></span>](http://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx)
  
[<span data-ttu-id="a0c77-174">Creating Contacts (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="a0c77-174">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="a0c77-175">Création de tâches</span><span class="sxs-lookup"><span data-stu-id="a0c77-175">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="a0c77-176">Création de rendez-vous</span><span class="sxs-lookup"><span data-stu-id="a0c77-176">Creating Appointments</span></span>](http://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

