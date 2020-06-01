---
title: GlobalLastDeliveryTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalLastDeliveryTime
api_type:
- schema
ms.assetid: a88dada9-c527-43a7-b2d3-31aad330def9
description: L’élément GlobalLastDeliveryTime contient le délai de remise du message qui a été reçu en dernier dans cette conversation sur tous les dossiers de la boîte aux lettres.
ms.openlocfilehash: b6d4d7c1d51c206e44973a717d25df4066845ada
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459411"
---
# <a name="globallastdeliverytime"></a><span data-ttu-id="65e2e-103">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="65e2e-103">GlobalLastDeliveryTime</span></span>

<span data-ttu-id="65e2e-104">L’élément **GlobalLastDeliveryTime** contient le délai de remise du message qui a été reçu en dernier dans cette conversation sur tous les dossiers de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="65e2e-104">The **GlobalLastDeliveryTime** element contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span> 
  
[<span data-ttu-id="65e2e-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="65e2e-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="65e2e-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="65e2e-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="65e2e-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="65e2e-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="65e2e-108">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="65e2e-108">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md)
  
```XML
<GlobalLastDeliveryTime/>
```

 <span data-ttu-id="65e2e-109">**XS : dateTime**</span><span class="sxs-lookup"><span data-stu-id="65e2e-109">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65e2e-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="65e2e-110">Attributes and elements</span></span>

<span data-ttu-id="65e2e-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="65e2e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65e2e-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="65e2e-112">Attributes</span></span>

<span data-ttu-id="65e2e-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="65e2e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65e2e-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="65e2e-114">Child elements</span></span>

<span data-ttu-id="65e2e-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="65e2e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="65e2e-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="65e2e-116">Parent elements</span></span>

|<span data-ttu-id="65e2e-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65e2e-117">**Element**</span></span>|<span data-ttu-id="65e2e-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="65e2e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65e2e-119">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="65e2e-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="65e2e-120">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="65e2e-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="65e2e-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="65e2e-121">Text value</span></span>

<span data-ttu-id="65e2e-122">La valeur de texte de l’élément **GlobalLastDeliveryTime** est la date et l’heure du dernier message reçu lors de cette conversation sur tous les dossiers de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="65e2e-122">The text value of the **GlobalLastDeliveryTime** element is the date and time of the message that was last received in this conversation across all folders in the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="65e2e-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="65e2e-123">Remarks</span></span>

<span data-ttu-id="65e2e-124">Cet élément a été introduit dans Exchange Server 2010 Service Pack 1 (SP1). Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="65e2e-124">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65e2e-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="65e2e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65e2e-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="65e2e-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="65e2e-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="65e2e-127">Schema name</span></span>  <br/> |<span data-ttu-id="65e2e-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="65e2e-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="65e2e-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="65e2e-129">Validation file</span></span>  <br/> |<span data-ttu-id="65e2e-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="65e2e-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="65e2e-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="65e2e-131">Can be empty</span></span>  <br/> |<span data-ttu-id="65e2e-132">False</span><span class="sxs-lookup"><span data-stu-id="65e2e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65e2e-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65e2e-133">See also</span></span>



[<span data-ttu-id="65e2e-134">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="65e2e-134">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="65e2e-135">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="65e2e-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="65e2e-136">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="65e2e-136">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

