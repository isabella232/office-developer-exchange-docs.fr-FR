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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462100"
---
# <a name="sendprompt"></a><span data-ttu-id="22c6e-103">SendPrompt</span><span class="sxs-lookup"><span data-stu-id="22c6e-103">SendPrompt</span></span>

<span data-ttu-id="22c6e-104">L’élément **SendPrompt** spécifie le type d’action autorisé pour une option de vote.</span><span class="sxs-lookup"><span data-stu-id="22c6e-104">The **SendPrompt** element specifies the type of action allowed for a voting option.</span></span> 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 <span data-ttu-id="22c6e-105">**SendPromptType**</span><span class="sxs-lookup"><span data-stu-id="22c6e-105">**SendPromptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22c6e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22c6e-106">Attributes and elements</span></span>

<span data-ttu-id="22c6e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22c6e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22c6e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="22c6e-108">Attributes</span></span>

<span data-ttu-id="22c6e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="22c6e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22c6e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22c6e-110">Child elements</span></span>

<span data-ttu-id="22c6e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="22c6e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="22c6e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22c6e-112">Parent elements</span></span>

[<span data-ttu-id="22c6e-113">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="22c6e-113">VotingOptionData</span></span>](votingoptiondata.md)
  
## <a name="text-value"></a><span data-ttu-id="22c6e-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="22c6e-114">Text value</span></span>

<span data-ttu-id="22c6e-115">La valeur de texte de l’élément **SendPrompt** est une action d’option de vote.</span><span class="sxs-lookup"><span data-stu-id="22c6e-115">The text value of the **SendPrompt** element is a voting option action.</span></span> <span data-ttu-id="22c6e-116">Le tableau suivant répertorie les valeurs possibles pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="22c6e-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="22c6e-117">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="22c6e-117">**Value**</span></span>|<span data-ttu-id="22c6e-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="22c6e-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="22c6e-119">Aucun</span><span class="sxs-lookup"><span data-stu-id="22c6e-119">None</span></span>  <br/> |<span data-ttu-id="22c6e-120">Aucune action.</span><span class="sxs-lookup"><span data-stu-id="22c6e-120">No action.</span></span>  <br/> |
|<span data-ttu-id="22c6e-121">Envoyer</span><span class="sxs-lookup"><span data-stu-id="22c6e-121">Send</span></span>  <br/> |<span data-ttu-id="22c6e-122">La réponse est envoyée immédiatement.</span><span class="sxs-lookup"><span data-stu-id="22c6e-122">The response is sent immediately.</span></span>  <br/> |
|<span data-ttu-id="22c6e-123">VotingOption</span><span class="sxs-lookup"><span data-stu-id="22c6e-123">VotingOption</span></span>  <br/> |<span data-ttu-id="22c6e-124">L’approbateur peut entrer des commentaires lors de l’approbation ou du rejet.</span><span class="sxs-lookup"><span data-stu-id="22c6e-124">The approver can enter comments while approving or rejecting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="22c6e-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="22c6e-125">Remarks</span></span>

<span data-ttu-id="22c6e-126">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="22c6e-126">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="22c6e-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="22c6e-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22c6e-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22c6e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22c6e-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22c6e-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22c6e-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22c6e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="22c6e-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="22c6e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="22c6e-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22c6e-132">Validation File</span></span>  <br/> |<span data-ttu-id="22c6e-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="22c6e-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="22c6e-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22c6e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="22c6e-135">True</span><span class="sxs-lookup"><span data-stu-id="22c6e-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22c6e-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22c6e-136">See also</span></span>



[<span data-ttu-id="22c6e-137">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="22c6e-137">VotingOptionData</span></span>](votingoptiondata.md)


- [<span data-ttu-id="22c6e-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="22c6e-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

