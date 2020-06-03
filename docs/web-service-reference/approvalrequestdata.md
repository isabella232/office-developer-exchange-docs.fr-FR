---
title: ApprovalRequestData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6c971cf7-5c3a-4e5e-9a7d-048f4ac0aadb
description: L’élément ApprovalRequestData spécifie l’état d’approbation d’un message de demande d’approbation.
ms.openlocfilehash: decbd4d646a56b9810387adcdb6a9049da89bc38
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462303"
---
# <a name="approvalrequestdata"></a><span data-ttu-id="14863-103">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="14863-103">ApprovalRequestData</span></span>

<span data-ttu-id="14863-104">L’élément **ApprovalRequestData** spécifie l’état d’approbation d’un message de demande d’approbation.</span><span class="sxs-lookup"><span data-stu-id="14863-104">The **ApprovalRequestData** element specifies the approval state of an approval request message.</span></span> 
  
```xml
<ApprovalRequestData>
   <IsUndecidedApprovalRequest/>
   <ApprovalDecision/>
   <ApprovalDecisionMaker/>
   <ApprovalDecisionTime/>
</ApprovalRequestData>
```

 <span data-ttu-id="14863-105">**ApprovalRequestDataType**</span><span class="sxs-lookup"><span data-stu-id="14863-105">**ApprovalRequestDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14863-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="14863-106">Attributes and elements</span></span>

<span data-ttu-id="14863-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="14863-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14863-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="14863-108">Attributes</span></span>

<span data-ttu-id="14863-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="14863-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14863-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="14863-110">Child elements</span></span>

<span data-ttu-id="14863-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md)  |  [ApprovalDecision](approvaldecision.md)  |  [ApprovalDecisionMaker](approvaldecisionmaker.md)  |  [ApprovalDecisionTime](approvaldecisiontime.md)</span><span class="sxs-lookup"><span data-stu-id="14863-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="14863-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="14863-112">Parent elements</span></span>

[<span data-ttu-id="14863-113">Message</span><span class="sxs-lookup"><span data-stu-id="14863-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="14863-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="14863-114">Remarks</span></span>

<span data-ttu-id="14863-115">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="14863-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="14863-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="14863-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14863-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="14863-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14863-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="14863-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="14863-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="14863-119">Schema Name</span></span>  <br/> |<span data-ttu-id="14863-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="14863-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="14863-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="14863-121">Validation File</span></span>  <br/> |<span data-ttu-id="14863-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="14863-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="14863-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="14863-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="14863-124">True</span><span class="sxs-lookup"><span data-stu-id="14863-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14863-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="14863-125">See also</span></span>

- [<span data-ttu-id="14863-126">Message</span><span class="sxs-lookup"><span data-stu-id="14863-126">Message</span></span>](message-ex15websvcsotherref.md)
- [<span data-ttu-id="14863-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="14863-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

