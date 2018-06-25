---
title: EnableAlwaysDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EnableAlwaysDelete
api_type:
- schema
ms.assetid: 7753aec5-3f93-4aeb-a28e-8b9b42ca7f9b
description: L’élément EnableAlwaysDelete spécifie un indicateur qui permet la suppression de tous les nouveaux éléments dans une conversation.
ms.openlocfilehash: f86765c641604afbf13ac962f4b34fbd8de56200
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756162"
---
# <a name="enablealwaysdelete"></a><span data-ttu-id="7d0a5-103">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="7d0a5-103">EnableAlwaysDelete</span></span>

<span data-ttu-id="7d0a5-104">L’élément **EnableAlwaysDelete** spécifie un indicateur qui permet la suppression de tous les nouveaux éléments dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="7d0a5-104">The **EnableAlwaysDelete** element specifies a flag that enables deletion for all new items in a conversation.</span></span> 
  
[<span data-ttu-id="7d0a5-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="7d0a5-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="7d0a5-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="7d0a5-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="7d0a5-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="7d0a5-107">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="7d0a5-108">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="7d0a5-108">EnableAlwaysDelete</span></span>](enablealwaysdelete.md)
  
```XML
<EnableAlwaysDelete/>
```

 <span data-ttu-id="7d0a5-109">**xs : Boolean**</span><span class="sxs-lookup"><span data-stu-id="7d0a5-109">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d0a5-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7d0a5-110">Attributes and elements</span></span>

<span data-ttu-id="7d0a5-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7d0a5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d0a5-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="7d0a5-112">Attributes</span></span>

<span data-ttu-id="7d0a5-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7d0a5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d0a5-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7d0a5-114">Child elements</span></span>

<span data-ttu-id="7d0a5-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7d0a5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d0a5-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7d0a5-116">Parent elements</span></span>

|<span data-ttu-id="7d0a5-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7d0a5-117">**Element**</span></span>|<span data-ttu-id="7d0a5-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d0a5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d0a5-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="7d0a5-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="7d0a5-120">Contient une seule action à appliquer à une même conversation.</span><span class="sxs-lookup"><span data-stu-id="7d0a5-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d0a5-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7d0a5-121">Text value</span></span>

<span data-ttu-id="7d0a5-122">La valeur de texte de l’élément **EnableAlwaysDelete** est **la valeur true** pour activer la suppression de tous les éléments de conversation ; Sinon, **false**.</span><span class="sxs-lookup"><span data-stu-id="7d0a5-122">The text value of the **EnableAlwaysDelete** element is **true** to enable the deletion of all items in conversation; otherwise, **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d0a5-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="7d0a5-123">Remarks</span></span>

<span data-ttu-id="7d0a5-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7d0a5-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d0a5-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7d0a5-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d0a5-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7d0a5-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7d0a5-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7d0a5-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7d0a5-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7d0a5-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="7d0a5-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7d0a5-129">Validation File</span></span>  <br/> |<span data-ttu-id="7d0a5-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7d0a5-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7d0a5-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7d0a5-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d0a5-132">False</span><span class="sxs-lookup"><span data-stu-id="7d0a5-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d0a5-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7d0a5-133">See also</span></span>



[<span data-ttu-id="7d0a5-134">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="7d0a5-134">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

