---
title: Actions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: L’élément Actions représente l’ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.
ms.openlocfilehash: 093d2f28135c6077b6cea488591573af0182934b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755156"
---
# <a name="actions"></a><span data-ttu-id="e6a98-103">Actions</span><span class="sxs-lookup"><span data-stu-id="e6a98-103">Actions</span></span>

<span data-ttu-id="e6a98-104">L’élément **Actions** représente l’ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="e6a98-104">The **Actions** element represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span> 
  
[<span data-ttu-id="e6a98-105">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="e6a98-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
```XML
<Actions>
    <AssignCategories>
    <CopyToFolder>
    <Delete>
    <ForwardAsAttachmentToRecipients>
    <ForwardToRecipients>
    <MarkImportance>
    <MarkAsRead>
    <MoveToFolder>
    <PermanentDelete>
    <RedirectToRecipients>
    <SendSMSAlertToRecipients>
    <ServerReplyWithMessage>
    <StopProcessingRules>
</Actions>
```

 <span data-ttu-id="e6a98-106">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="e6a98-106">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6a98-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e6a98-107">Attributes and elements</span></span>

<span data-ttu-id="e6a98-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e6a98-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6a98-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="e6a98-109">Attributes</span></span>

<span data-ttu-id="e6a98-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e6a98-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6a98-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e6a98-111">Child elements</span></span>

|<span data-ttu-id="e6a98-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e6a98-112">**Element**</span></span>|<span data-ttu-id="e6a98-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="e6a98-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6a98-114">AssignCategories</span><span class="sxs-lookup"><span data-stu-id="e6a98-114">AssignCategories</span></span>](assigncategories.md) <br/> |<span data-ttu-id="e6a98-115">Représente les catégories qui sont marqués dans les messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="e6a98-115">Represents the categories that are stamped on e-mail messages.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-116">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="e6a98-116">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="e6a98-117">Identifie l’ID du dossier qui sont copiées dans les éléments de courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="e6a98-117">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-118">Supprimer</span><span class="sxs-lookup"><span data-stu-id="e6a98-118">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="e6a98-119">Indique si les messages doivent être déplacés vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="e6a98-119">Indicates whether messages are to be moved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-120">ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="e6a98-120">ForwardAsAttachmentToRecipients</span></span>](forwardasattachmenttorecipients.md) <br/> |<span data-ttu-id="e6a98-121">Indique les adresses de messagerie à laquelle les messages sont transmis en tant que pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="e6a98-121">Indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-122">ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="e6a98-122">ForwardToRecipients</span></span>](forwardtorecipients.md) <br/> |<span data-ttu-id="e6a98-123">Indique les adresses de messagerie à laquelle les messages doivent être transférés.</span><span class="sxs-lookup"><span data-stu-id="e6a98-123">Indicates the e-mail addresses to which messages are to be forwarded.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-124">MarkImportance</span><span class="sxs-lookup"><span data-stu-id="e6a98-124">MarkImportance</span></span>](markimportance.md) <br/> |<span data-ttu-id="e6a98-125">Spécifie l’importance qui doit être marqué sur les messages.</span><span class="sxs-lookup"><span data-stu-id="e6a98-125">Specifies the importance that is to be stamped on messages.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-126">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="e6a98-126">MarkAsRead</span></span>](markasread.md) <br/> |<span data-ttu-id="e6a98-127">Indique si les messages doivent être marqués comme étant en lecture.</span><span class="sxs-lookup"><span data-stu-id="e6a98-127">Indicates whether messages are to be marked as read.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-128">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="e6a98-128">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="e6a98-129">Identifie l’ID du dossier qui seront déplacées vers des éléments de courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="e6a98-129">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-130">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="e6a98-130">PermanentDelete</span></span>](permanentdelete.md) <br/> |<span data-ttu-id="e6a98-131">Indique si les messages doivent être définitivement supprimés et non enregistré dans le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="e6a98-131">Indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-132">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="e6a98-132">RedirectToRecipients</span></span>](redirecttorecipients.md) <br/> |<span data-ttu-id="e6a98-133">Indique les adresses de messagerie à laquelle les messages doivent être redirigé.</span><span class="sxs-lookup"><span data-stu-id="e6a98-133">Indicates the e-mail addresses to which messages are to be redirected.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-134">SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="e6a98-134">SendSMSAlertToRecipients</span></span>](sendsmsalerttorecipients.md) <br/> |<span data-ttu-id="e6a98-135">Indique les numéros de téléphone mobile à laquelle une alerte Service SMS (Short Message) doit être envoyé.</span><span class="sxs-lookup"><span data-stu-id="e6a98-135">Indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-136">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="e6a98-136">ServerReplyWithMessage</span></span>](serverreplywithmessage.md) <br/> |<span data-ttu-id="e6a98-137">Indique.</span><span class="sxs-lookup"><span data-stu-id="e6a98-137">Indicates.</span></span> <span data-ttu-id="e6a98-138">ID de modèle de message qui doit être envoyé en réponse aux messages entrants.</span><span class="sxs-lookup"><span data-stu-id="e6a98-138">the ID of the template message that is to be sent as a reply to incoming messages.</span></span>  <br/> |
|[<span data-ttu-id="e6a98-139">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="e6a98-139">StopProcessingRules</span></span>](stopprocessingrules.md) <br/> |<span data-ttu-id="e6a98-140">Indique si les règles suivantes doivent être évaluées.</span><span class="sxs-lookup"><span data-stu-id="e6a98-140">Indicates whether subsequent rules are to be evaluated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e6a98-141">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e6a98-141">Parent elements</span></span>

|<span data-ttu-id="e6a98-142">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e6a98-142">**Element**</span></span>|<span data-ttu-id="e6a98-143">**Description**</span><span class="sxs-lookup"><span data-stu-id="e6a98-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6a98-144">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="e6a98-144">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="e6a98-145">Représente une règle de boîte aux lettres d’un utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="e6a98-145">Represents a single rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e6a98-146">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e6a98-146">Text value</span></span>

<span data-ttu-id="e6a98-147">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e6a98-147">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e6a98-148">Remarques</span><span class="sxs-lookup"><span data-stu-id="e6a98-148">Remarks</span></span>

<span data-ttu-id="e6a98-149">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6a98-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6a98-150">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e6a98-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6a98-151">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e6a98-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e6a98-152">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e6a98-152">Schema Name</span></span>  <br/> |<span data-ttu-id="e6a98-153">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e6a98-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="e6a98-154">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e6a98-154">Validation File</span></span>  <br/> |<span data-ttu-id="e6a98-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e6a98-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e6a98-156">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e6a98-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6a98-157">True</span><span class="sxs-lookup"><span data-stu-id="e6a98-157">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6a98-158">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e6a98-158">See also</span></span>

- [<span data-ttu-id="e6a98-159">Conditions</span><span class="sxs-lookup"><span data-stu-id="e6a98-159">Conditions</span></span>](conditions.md)
- [<span data-ttu-id="e6a98-160">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e6a98-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
