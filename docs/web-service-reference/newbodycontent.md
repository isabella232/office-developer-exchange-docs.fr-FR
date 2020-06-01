---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: L’élément NewBodyContent représente le nouveau contenu du corps d’un message.
ms.openlocfilehash: dcfa927bb284ff00e510d8c7b4b31910a70b3cbb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466856"
---
# <a name="newbodycontent"></a><span data-ttu-id="79967-103">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="79967-103">NewBodyContent</span></span>

<span data-ttu-id="79967-104">L’élément **NewBodyContent** représente le nouveau contenu du corps d’un message.</span><span class="sxs-lookup"><span data-stu-id="79967-104">The **NewBodyContent** element represents the new body content of a message.</span></span> 
  
```xml
<NewBodyContent BodyType=""/>
```

 <span data-ttu-id="79967-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="79967-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79967-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="79967-106">Attributes and elements</span></span>

<span data-ttu-id="79967-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="79967-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79967-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="79967-108">Attributes</span></span>

|<span data-ttu-id="79967-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="79967-109">**Attribute**</span></span>|<span data-ttu-id="79967-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="79967-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="79967-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="79967-111">**BodyType**</span></span> <br/> |<span data-ttu-id="79967-112">Représente le contenu réel du corps d'un message.</span><span class="sxs-lookup"><span data-stu-id="79967-112">Represents the actual body content of a message.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="79967-113">Attribut BodyType</span><span class="sxs-lookup"><span data-stu-id="79967-113">BodyType Attribute</span></span>

|<span data-ttu-id="79967-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="79967-114">**Value**</span></span>|<span data-ttu-id="79967-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="79967-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="79967-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="79967-116">**HTML**</span></span> <br/> |<span data-ttu-id="79967-117">Convertit tous les corps au format HTML.</span><span class="sxs-lookup"><span data-stu-id="79967-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="79967-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="79967-118">**Text**</span></span> <br/> |<span data-ttu-id="79967-119">Convertit tous les corps en texte brut.</span><span class="sxs-lookup"><span data-stu-id="79967-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="79967-120">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="79967-120">Child elements</span></span>

<span data-ttu-id="79967-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79967-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79967-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="79967-122">Parent elements</span></span>

|<span data-ttu-id="79967-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79967-123">**Element**</span></span>|<span data-ttu-id="79967-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="79967-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79967-125">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="79967-125">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="79967-126">Contient une réponse à l’expéditeur d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="79967-126">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79967-127">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="79967-127">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="79967-128">Contient une réponse à l’expéditeur et à tous les destinataires identifiés d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="79967-128">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79967-129">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="79967-129">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="79967-130">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="79967-130">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="79967-131">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="79967-131">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="79967-132">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="79967-132">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="79967-133">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="79967-133">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="79967-134">Contient une réponse à un élément de publication.</span><span class="sxs-lookup"><span data-stu-id="79967-134">Contains a reply to a post item.</span></span> <span data-ttu-id="79967-135">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="79967-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79967-136">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="79967-136">Text value</span></span>

<span data-ttu-id="79967-137">La valeur de texte représente le nouveau contenu du corps d’un message.</span><span class="sxs-lookup"><span data-stu-id="79967-137">The text value represents the new body content of a message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79967-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="79967-138">Remarks</span></span>

<span data-ttu-id="79967-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS du serveur Exchange sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="79967-139">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79967-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="79967-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79967-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="79967-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79967-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="79967-142">Schema Name</span></span>  <br/> |<span data-ttu-id="79967-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="79967-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="79967-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="79967-144">Validation File</span></span>  <br/> |<span data-ttu-id="79967-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="79967-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79967-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="79967-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="79967-147">False</span><span class="sxs-lookup"><span data-stu-id="79967-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79967-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79967-148">See also</span></span>



- [<span data-ttu-id="79967-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="79967-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

