---
title: ApprovalDecision
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e7c5687-cb9e-4f0b-ac8f-b82591914a39
description: L’élément ApprovalDecision spécifie la décision prise sur un message de demande d’approbation.
ms.openlocfilehash: a8dc168edec882ba97cdea764f8d20c71ed85f8a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463446"
---
# <a name="approvaldecision"></a><span data-ttu-id="0aadc-103">ApprovalDecision</span><span class="sxs-lookup"><span data-stu-id="0aadc-103">ApprovalDecision</span></span>

<span data-ttu-id="0aadc-104">L’élément **ApprovalDecision** spécifie la décision prise sur un message de demande d’approbation.</span><span class="sxs-lookup"><span data-stu-id="0aadc-104">The **ApprovalDecision** element specifies the decision made on an approval request message.</span></span> 
  
```XML
<ApprovalDecision> 1 | 2 </ApprovalDecision>
```

 <span data-ttu-id="0aadc-105">**int**</span><span class="sxs-lookup"><span data-stu-id="0aadc-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0aadc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0aadc-106">Attributes and elements</span></span>

<span data-ttu-id="0aadc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0aadc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0aadc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0aadc-108">Attributes</span></span>

<span data-ttu-id="0aadc-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0aadc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0aadc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0aadc-110">Child elements</span></span>

<span data-ttu-id="0aadc-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0aadc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0aadc-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0aadc-112">Parent elements</span></span>

[<span data-ttu-id="0aadc-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="0aadc-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="0aadc-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0aadc-114">Text value</span></span>

<span data-ttu-id="0aadc-115">La valeur de texte de l’élément **ApprovalDecision** est 1 si approuvé et 2 si rejeté.</span><span class="sxs-lookup"><span data-stu-id="0aadc-115">The text value of the **ApprovalDecision** element is 1 if approved and 2 if rejected.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0aadc-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="0aadc-116">Remarks</span></span>

<span data-ttu-id="0aadc-117">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0aadc-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="0aadc-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0aadc-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0aadc-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0aadc-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0aadc-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0aadc-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0aadc-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0aadc-121">Schema Name</span></span>  <br/> |<span data-ttu-id="0aadc-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0aadc-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="0aadc-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0aadc-123">Validation File</span></span>  <br/> |<span data-ttu-id="0aadc-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0aadc-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0aadc-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0aadc-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="0aadc-126">True</span><span class="sxs-lookup"><span data-stu-id="0aadc-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0aadc-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0aadc-127">See also</span></span>

- [<span data-ttu-id="0aadc-128">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="0aadc-128">ApprovalRequestData</span></span>](approvalrequestdata.md)
- [<span data-ttu-id="0aadc-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0aadc-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

