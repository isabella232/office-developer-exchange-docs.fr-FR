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
description: L’élément CreateItem définit une demande de création d’un élément dans la Banque d’Exchange.
ms.openlocfilehash: 235664b7baeceeccb14135fd346123f0f7d99346
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527060"
---
# <a name="createitem"></a><span data-ttu-id="b11eb-103">CreateItem</span><span class="sxs-lookup"><span data-stu-id="b11eb-103">CreateItem</span></span>

<span data-ttu-id="b11eb-104">L’élément **CreateItem** définit une demande de création d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="b11eb-104">The **CreateItem** element defines a request to create an item in the Exchange store.</span></span> 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

<span data-ttu-id="b11eb-105">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="b11eb-105">**CreateItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b11eb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b11eb-106">Attributes and elements</span></span>

<span data-ttu-id="b11eb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b11eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b11eb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b11eb-108">Attributes</span></span>

|<span data-ttu-id="b11eb-109">Attribut</span><span class="sxs-lookup"><span data-stu-id="b11eb-109">Attribute</span></span>|<span data-ttu-id="b11eb-110">Description</span><span class="sxs-lookup"><span data-stu-id="b11eb-110">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="b11eb-111">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="b11eb-111">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="b11eb-112">Indique comment l’élément sera géré après sa création.</span><span class="sxs-lookup"><span data-stu-id="b11eb-112">Describes how the item will be handled after it is created.</span></span> <span data-ttu-id="b11eb-113">L’attribut est requis pour les messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="b11eb-113">The attribute is required for e-mail messages.</span></span> <span data-ttu-id="b11eb-114">Cet attribut n’est applicable qu’aux messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="b11eb-114">This attribute is only applicable to e-mail messages.</span></span>  <br/> |
|<span data-ttu-id="b11eb-115">**SendMeetingInvitations**</span><span class="sxs-lookup"><span data-stu-id="b11eb-115">**SendMeetingInvitations**</span></span> <br/> |<span data-ttu-id="b11eb-116">Décrit comment les demandes de réunion sont gérées après leur création.</span><span class="sxs-lookup"><span data-stu-id="b11eb-116">Describes how meeting requests are handled after they are created.</span></span> <span data-ttu-id="b11eb-117">Cet attribut est requis pour les éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="b11eb-117">This attribute is required for calendar items.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="b11eb-118">Attribut MessageDisposition</span><span class="sxs-lookup"><span data-stu-id="b11eb-118">MessageDisposition Attribute</span></span>

|<span data-ttu-id="b11eb-119">Valeur</span><span class="sxs-lookup"><span data-stu-id="b11eb-119">Value</span></span>|<span data-ttu-id="b11eb-120">Description</span><span class="sxs-lookup"><span data-stu-id="b11eb-120">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="b11eb-121">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="b11eb-121">SaveOnly</span></span>  <br/> |<span data-ttu-id="b11eb-122">L’élément de message est enregistré dans le dossier spécifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="b11eb-122">The message item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="b11eb-123">Les messages peuvent être envoyés ultérieurement à l’aide de l' [opération SendItem](senditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b11eb-123">Messages can be sent later by using the [SendItem operation](senditem-operation.md).</span></span> <span data-ttu-id="b11eb-124">Un identificateur d’élément est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b11eb-124">An item identifier is returned in the response.</span></span> <span data-ttu-id="b11eb-125">Les identificateurs d’élément ne sont renvoyés pour aucun type d’élément, à l’exception des éléments de message.</span><span class="sxs-lookup"><span data-stu-id="b11eb-125">Item identifiers are not returned for any item types except for message items.</span></span> <span data-ttu-id="b11eb-126">Cela inclut les objets Response.</span><span class="sxs-lookup"><span data-stu-id="b11eb-126">This includes response objects.</span></span>  <br/> |
|<span data-ttu-id="b11eb-127">SendOnly</span><span class="sxs-lookup"><span data-stu-id="b11eb-127">SendOnly</span></span>  <br/> |<span data-ttu-id="b11eb-128">L’élément est envoyé, mais aucune copie n’est enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="b11eb-128">The item is sent but no copy is saved in the Sent Items folder.</span></span> <span data-ttu-id="b11eb-129">Un identificateur d’élément n’est pas renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b11eb-129">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="b11eb-130">**Remarque**: **CreateItem** ne prend pas en charge l’accès délégué lorsque l’option SendOnly est utilisée, car un dossier de destination ne peut pas être spécifié avec cette option.</span><span class="sxs-lookup"><span data-stu-id="b11eb-130">**NOTE**: **CreateItem** does not support delegate access when the SendOnly option is used because a destination folder cannot be specified with this option.</span></span> <span data-ttu-id="b11eb-131">La solution de contournement consiste à créer l’élément, à obtenir l’identificateur de l’élément, puis à utiliser l’opération SendItem pour envoyer l’élément.</span><span class="sxs-lookup"><span data-stu-id="b11eb-131">The workaround is to create the item, get the item identifier, and then use the SendItem operation to send the item.</span></span>           |
|<span data-ttu-id="b11eb-132">Méthodesendandsavecopy</span><span class="sxs-lookup"><span data-stu-id="b11eb-132">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="b11eb-133">L’élément est envoyé et une copie est enregistrée dans le dossier qui est identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="b11eb-133">The item is sent and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="b11eb-134">Un identificateur d’élément n’est pas renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b11eb-134">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="b11eb-135">**Remarque**: les demandes de réunion ne sont pas enregistrées dans le dossier qui est identifié par la propriété [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="b11eb-135">**NOTE**: Meeting requests are not saved to the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) property.</span></span> <span data-ttu-id="b11eb-136">Pour le calendrier, seul l’emplacement d’enregistrement des éléments de calendrier peut être spécifié par la propriété **SavedItemFolderId** .</span><span class="sxs-lookup"><span data-stu-id="b11eb-136">For calendaring, only the save location for calendar items can be specified by the **SavedItemFolderId** property.</span></span> <span data-ttu-id="b11eb-137">Vous ne pouvez pas contrôler l’emplacement d’enregistrement d’un élément de demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="b11eb-137">You cannot control where a meeting request item is saved.</span></span> <span data-ttu-id="b11eb-138">Seuls les éléments de calendrier associés sont copiés et enregistrés dans le dossier qui est identifié par la propriété **SavedItemFolderId** .</span><span class="sxs-lookup"><span data-stu-id="b11eb-138">Only the associated calendar items are copied and saved into the folder that is identified by the **SavedItemFolderId** property.</span></span>           |
   
#### <a name="sendmeetinginvitations-attribute"></a><span data-ttu-id="b11eb-139">Attribut SendMeetingInvitations</span><span class="sxs-lookup"><span data-stu-id="b11eb-139">SendMeetingInvitations Attribute</span></span>

|<span data-ttu-id="b11eb-140">Valeur</span><span class="sxs-lookup"><span data-stu-id="b11eb-140">Value</span></span>|<span data-ttu-id="b11eb-141">Description</span><span class="sxs-lookup"><span data-stu-id="b11eb-141">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="b11eb-142">SendToNone</span><span class="sxs-lookup"><span data-stu-id="b11eb-142">SendToNone</span></span>  <br/> |<span data-ttu-id="b11eb-143">Si l’élément est une demande de réunion, il est enregistré en tant qu’élément de calendrier mais pas envoyé.</span><span class="sxs-lookup"><span data-stu-id="b11eb-143">If the item is a meeting request, it is saved as a calendar item but not sent.</span></span>  <br/> |
|<span data-ttu-id="b11eb-144">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="b11eb-144">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="b11eb-145">La demande de réunion est envoyée à tous les participants, mais n’est pas enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="b11eb-145">The meeting request is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="b11eb-146">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="b11eb-146">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="b11eb-147">La demande de réunion est envoyée à tous les participants et une copie est enregistrée dans le dossier qui est identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="b11eb-147">The meeting request is sent to all attendees and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b11eb-148">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b11eb-148">Child elements</span></span>

|<span data-ttu-id="b11eb-149">Élément</span><span class="sxs-lookup"><span data-stu-id="b11eb-149">Element</span></span>|<span data-ttu-id="b11eb-150">Description</span><span class="sxs-lookup"><span data-stu-id="b11eb-150">Description</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b11eb-151">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="b11eb-151">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="b11eb-152">Identifie le dossier cible dans lequel un nouvel élément peut être créé.</span><span class="sxs-lookup"><span data-stu-id="b11eb-152">Identifies the target folder where a new item can be created.</span></span> <span data-ttu-id="b11eb-153">Si l’attribut **MessageDisposition** est défini sur SendOnly, un message créé sera uniquement envoyé.</span><span class="sxs-lookup"><span data-stu-id="b11eb-153">If the **MessageDisposition** attribute is set to SendOnly, a created message will only be sent.</span></span> <span data-ttu-id="b11eb-154">Le message ne sera pas placé dans le dossier qui est identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="b11eb-154">The message will not be put in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="b11eb-155">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="b11eb-155">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="b11eb-156">Contient un tableau d’éléments à créer dans le dossier qui est identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="b11eb-156">Contains an array of items to create in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b11eb-157">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b11eb-157">Parent elements</span></span>

<span data-ttu-id="b11eb-158">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b11eb-158">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b11eb-159">Remarques</span><span class="sxs-lookup"><span data-stu-id="b11eb-159">Remarks</span></span>

<span data-ttu-id="b11eb-160">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b11eb-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b11eb-161">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b11eb-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b11eb-162">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b11eb-162">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b11eb-163">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b11eb-163">Schema Name</span></span>  <br/> |<span data-ttu-id="b11eb-164">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b11eb-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b11eb-165">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b11eb-165">Validation File</span></span>  <br/> |<span data-ttu-id="b11eb-166">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b11eb-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b11eb-167">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b11eb-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="b11eb-168">False</span><span class="sxs-lookup"><span data-stu-id="b11eb-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b11eb-169">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b11eb-169">See also</span></span>

- [<span data-ttu-id="b11eb-170">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="b11eb-170">CreateItemResponse</span></span>](createitemresponse.md)  
- [<span data-ttu-id="b11eb-171">Opération CreateItem</span><span class="sxs-lookup"><span data-stu-id="b11eb-171">CreateItem operation</span></span>](createitem-operation.md)
- [<span data-ttu-id="b11eb-172">Création de messages électroniques</span><span class="sxs-lookup"><span data-stu-id="b11eb-172">Creating E-mail Messages</span></span>](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [<span data-ttu-id="b11eb-173">Creating Contacts (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="b11eb-173">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="b11eb-174">Création de tâches</span><span class="sxs-lookup"><span data-stu-id="b11eb-174">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [<span data-ttu-id="b11eb-175">Création de rendez-vous</span><span class="sxs-lookup"><span data-stu-id="b11eb-175">Creating Appointments</span></span>](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

