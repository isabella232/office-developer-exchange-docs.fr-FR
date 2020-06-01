---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: L’élément SendPrompt spécifie le type d’action autorisé pour une option de vote.
ms.openlocfilehash: 98ffc69cdc94c3f7b9c325bee0c1ebaeb407ee96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462100"
---
# <a name="sendprompt"></a><span data-ttu-id="88846-103">SendPrompt</span><span class="sxs-lookup"><span data-stu-id="88846-103">SendPrompt</span></span>

<span data-ttu-id="88846-104">L’élément **SendPrompt** spécifie le type d’action autorisé pour une option de vote.</span><span class="sxs-lookup"><span data-stu-id="88846-104">The **SendPrompt** element specifies the type of action allowed for a voting option.</span></span> 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 <span data-ttu-id="88846-105">**SendPromptType**</span><span class="sxs-lookup"><span data-stu-id="88846-105">**SendPromptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88846-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="88846-106">Attributes and elements</span></span>

<span data-ttu-id="88846-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="88846-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88846-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="88846-108">Attributes</span></span>

<span data-ttu-id="88846-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="88846-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88846-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="88846-110">Child elements</span></span>

<span data-ttu-id="88846-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="88846-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="88846-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="88846-112">Parent elements</span></span>

[<span data-ttu-id="88846-113">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="88846-113">VotingOptionData</span></span>](votingoptiondata.md)
  
## <a name="text-value"></a><span data-ttu-id="88846-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="88846-114">Text value</span></span>

<span data-ttu-id="88846-115">La valeur de texte de l’élément **SendPrompt** est une action d’option de vote.</span><span class="sxs-lookup"><span data-stu-id="88846-115">The text value of the **SendPrompt** element is a voting option action.</span></span> <span data-ttu-id="88846-116">Le tableau suivant répertorie les valeurs possibles pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="88846-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="88846-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="88846-117">**Value**</span></span>|<span data-ttu-id="88846-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="88846-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="88846-119">Aucun</span><span class="sxs-lookup"><span data-stu-id="88846-119">None</span></span>  <br/> |<span data-ttu-id="88846-120">Aucune action.</span><span class="sxs-lookup"><span data-stu-id="88846-120">No action.</span></span>  <br/> |
|<span data-ttu-id="88846-121">Envoyer</span><span class="sxs-lookup"><span data-stu-id="88846-121">Send</span></span>  <br/> |<span data-ttu-id="88846-122">La réponse est envoyée immédiatement.</span><span class="sxs-lookup"><span data-stu-id="88846-122">The response is sent immediately.</span></span>  <br/> |
|<span data-ttu-id="88846-123">VotingOption</span><span class="sxs-lookup"><span data-stu-id="88846-123">VotingOption</span></span>  <br/> |<span data-ttu-id="88846-124">L’approbateur peut entrer des commentaires lors de l’approbation ou du rejet.</span><span class="sxs-lookup"><span data-stu-id="88846-124">The approver can enter comments while approving or rejecting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="88846-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="88846-125">Remarks</span></span>

<span data-ttu-id="88846-126">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="88846-126">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="88846-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="88846-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88846-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="88846-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88846-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="88846-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88846-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="88846-130">Schema Name</span></span>  <br/> |<span data-ttu-id="88846-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="88846-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="88846-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="88846-132">Validation File</span></span>  <br/> |<span data-ttu-id="88846-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="88846-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88846-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="88846-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="88846-135">True</span><span class="sxs-lookup"><span data-stu-id="88846-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88846-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="88846-136">See also</span></span>



[<span data-ttu-id="88846-137">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="88846-137">VotingOptionData</span></span>](votingoptiondata.md)


- [<span data-ttu-id="88846-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="88846-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

