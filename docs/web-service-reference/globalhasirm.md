---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: L’élément GlobalHasIrm indique si au moins un message dans la conversation et sur tous les dossiers est un message protégé IRM.
ms.openlocfilehash: ad3eafcb38829e7ea57cbc7535b0f5411ad595d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827717"
---
# <a name="globalhasirm"></a><span data-ttu-id="f6b13-103">GlobalHasIrm</span><span class="sxs-lookup"><span data-stu-id="f6b13-103">GlobalHasIrm</span></span>

<span data-ttu-id="f6b13-104">L’élément **GlobalHasIrm** indique si au moins un message dans la conversation et sur tous les dossiers est un message protégé IRM.</span><span class="sxs-lookup"><span data-stu-id="f6b13-104">The **GlobalHasIrm** element specifies whether at least one message in the conversation and across all folders is an IRM protected message.</span></span> 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 <span data-ttu-id="f6b13-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f6b13-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6b13-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f6b13-106">Attributes and elements</span></span>

<span data-ttu-id="f6b13-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f6b13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6b13-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f6b13-108">Attributes</span></span>

<span data-ttu-id="f6b13-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f6b13-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6b13-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f6b13-110">Child elements</span></span>

<span data-ttu-id="f6b13-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f6b13-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f6b13-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f6b13-112">Parent elements</span></span>

[<span data-ttu-id="f6b13-113">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f6b13-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="f6b13-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f6b13-114">Text value</span></span>

<span data-ttu-id="f6b13-115">La valeur de texte de l’élément **GlobalHasIrm** est **la valeur true** si au moins un message dans la conversation et sur tous les dossiers est un message protégé IRM.</span><span class="sxs-lookup"><span data-stu-id="f6b13-115">The text value of the **GlobalHasIrm** element is **true** if at least one message in the conversation and across all folders is an IRM protected message.</span></span> <span data-ttu-id="f6b13-116">Dans le cas contraire, la valeur est **false**.</span><span class="sxs-lookup"><span data-stu-id="f6b13-116">Otherwise the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f6b13-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="f6b13-117">Remarks</span></span>

<span data-ttu-id="f6b13-118">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f6b13-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="f6b13-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6b13-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6b13-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f6b13-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6b13-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f6b13-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f6b13-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f6b13-122">Schema Name</span></span>  <br/> |<span data-ttu-id="f6b13-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f6b13-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="f6b13-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f6b13-124">Validation File</span></span>  <br/> |<span data-ttu-id="f6b13-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f6b13-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f6b13-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f6b13-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6b13-127">True</span><span class="sxs-lookup"><span data-stu-id="f6b13-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6b13-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f6b13-128">See also</span></span>



[<span data-ttu-id="f6b13-129">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f6b13-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="f6b13-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f6b13-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

