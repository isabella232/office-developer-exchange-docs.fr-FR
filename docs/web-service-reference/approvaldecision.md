---
title: ApprovalDecision
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e7c5687-cb9e-4f0b-ac8f-b82591914a39
description: L’élément ApprovalDecision spécifie la décision sur un message de demande d’approbation.
ms.openlocfilehash: 4ca73813440200e5d2fb9f920d81459d8cd5e4ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755305"
---
# <a name="approvaldecision"></a><span data-ttu-id="0928f-103">ApprovalDecision</span><span class="sxs-lookup"><span data-stu-id="0928f-103">ApprovalDecision</span></span>

<span data-ttu-id="0928f-104">L’élément **ApprovalDecision** spécifie la décision sur un message de demande d’approbation.</span><span class="sxs-lookup"><span data-stu-id="0928f-104">The **ApprovalDecision** element specifies the decision made on an approval request message.</span></span> 
  
```XML
<ApprovalDecision> 1 | 2 </ApprovalDecision>
```

 <span data-ttu-id="0928f-105">**int**</span><span class="sxs-lookup"><span data-stu-id="0928f-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0928f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0928f-106">Attributes and elements</span></span>

<span data-ttu-id="0928f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0928f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0928f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0928f-108">Attributes</span></span>

<span data-ttu-id="0928f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0928f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0928f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0928f-110">Child elements</span></span>

<span data-ttu-id="0928f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0928f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0928f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0928f-112">Parent elements</span></span>

[<span data-ttu-id="0928f-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="0928f-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="0928f-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0928f-114">Text value</span></span>

<span data-ttu-id="0928f-115">La valeur de texte de l’élément **ApprovalDecision** est 1 si approuvé et 2 si rejeté.</span><span class="sxs-lookup"><span data-stu-id="0928f-115">The text value of the **ApprovalDecision** element is 1 if approved and 2 if rejected.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0928f-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="0928f-116">Remarks</span></span>

<span data-ttu-id="0928f-117">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0928f-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="0928f-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0928f-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0928f-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0928f-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0928f-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0928f-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0928f-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0928f-121">Schema Name</span></span>  <br/> |<span data-ttu-id="0928f-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0928f-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="0928f-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0928f-123">Validation File</span></span>  <br/> |<span data-ttu-id="0928f-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0928f-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0928f-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0928f-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="0928f-126">True</span><span class="sxs-lookup"><span data-stu-id="0928f-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0928f-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0928f-127">See also</span></span>

- [<span data-ttu-id="0928f-128">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="0928f-128">ApprovalRequestData</span></span>](approvalrequestdata.md)
- [<span data-ttu-id="0928f-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0928f-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

