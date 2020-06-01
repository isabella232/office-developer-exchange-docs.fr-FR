---
title: LastDeliveryTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LastDeliveryTime
api_type:
- schema
ms.assetid: 23d02ceb-f28e-40f2-8f63-673723a50e2a
description: L’élément LastDeliveryTime contient le délai de remise du message qui a été reçu en dernier dans cette conversation dans le dossier actif.
ms.openlocfilehash: 77147693a9394e983575afa6fcfda242f8f76ae3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458109"
---
# <a name="lastdeliverytime"></a><span data-ttu-id="671f9-103">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="671f9-103">LastDeliveryTime</span></span>

<span data-ttu-id="671f9-104">L’élément **LastDeliveryTime** contient le délai de remise du message qui a été reçu en dernier dans cette conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="671f9-104">The **LastDeliveryTime** element contains the delivery time of the message that was last received in this conversation in the current folder.</span></span> 
  
[<span data-ttu-id="671f9-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="671f9-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="671f9-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="671f9-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="671f9-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="671f9-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="671f9-108">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="671f9-108">LastDeliveryTime</span></span>](lastdeliverytime.md)
  
```XML
<LastDeliveryTime/>
```

 <span data-ttu-id="671f9-109">**XS : dateTime**</span><span class="sxs-lookup"><span data-stu-id="671f9-109">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="671f9-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="671f9-110">Attributes and elements</span></span>

<span data-ttu-id="671f9-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="671f9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="671f9-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="671f9-112">Attributes</span></span>

<span data-ttu-id="671f9-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="671f9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="671f9-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="671f9-114">Child elements</span></span>

<span data-ttu-id="671f9-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="671f9-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="671f9-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="671f9-116">Parent elements</span></span>

|<span data-ttu-id="671f9-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="671f9-117">**Element**</span></span>|<span data-ttu-id="671f9-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="671f9-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="671f9-119">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="671f9-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="671f9-120">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="671f9-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="671f9-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="671f9-121">Text value</span></span>

<span data-ttu-id="671f9-122">La valeur de texte de l’élément **LastDeliveryTime** est la date et l’heure du dernier message reçu dans cette conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="671f9-122">The text value of the **LastDeliveryTime** element is the date and time of the message that was last received in this conversation in the current folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="671f9-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="671f9-123">Remarks</span></span>

<span data-ttu-id="671f9-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="671f9-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="671f9-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="671f9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="671f9-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="671f9-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="671f9-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="671f9-127">Schema name</span></span>  <br/> |<span data-ttu-id="671f9-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="671f9-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="671f9-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="671f9-129">Validation file</span></span>  <br/> |<span data-ttu-id="671f9-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="671f9-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="671f9-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="671f9-131">Can be empty</span></span>  <br/> |<span data-ttu-id="671f9-132">False</span><span class="sxs-lookup"><span data-stu-id="671f9-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="671f9-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="671f9-133">See also</span></span>



[<span data-ttu-id="671f9-134">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="671f9-134">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="671f9-135">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="671f9-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="671f9-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="671f9-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="671f9-137">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="671f9-137">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

