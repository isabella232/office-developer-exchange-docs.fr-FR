---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: L’élément IsUndecidedApprovalRequest Spécifie si un message de demande d’approbation a été effectuée.
ms.openlocfilehash: 82b4624df5b2fe7ca212fdf76248e1ccfa3a081f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828127"
---
# <a name="isundecidedapprovalrequest"></a><span data-ttu-id="117b2-103">IsUndecidedApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="117b2-103">IsUndecidedApprovalRequest</span></span>

<span data-ttu-id="117b2-104">L’élément **IsUndecidedApprovalRequest** Spécifie si un message de demande d’approbation a été effectuée.</span><span class="sxs-lookup"><span data-stu-id="117b2-104">The **IsUndecidedApprovalRequest** element specifies whether an approval request message has been acted on.</span></span> 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 <span data-ttu-id="117b2-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="117b2-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="117b2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="117b2-106">Attributes and elements</span></span>

<span data-ttu-id="117b2-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="117b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="117b2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="117b2-108">Attributes</span></span>

<span data-ttu-id="117b2-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="117b2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="117b2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="117b2-110">Child elements</span></span>

<span data-ttu-id="117b2-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="117b2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="117b2-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="117b2-112">Parent elements</span></span>

[<span data-ttu-id="117b2-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="117b2-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="117b2-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="117b2-114">Text value</span></span>

<span data-ttu-id="117b2-115">La valeur de texte de l’élément **IsUndecidedApprovalRequest** est **la valeur true** si un message de demande d’approbation n’a pas été effectuée.</span><span class="sxs-lookup"><span data-stu-id="117b2-115">The text value of the **IsUndecidedApprovalRequest** element is **true** if an approval request message has not been acted on.</span></span> <span data-ttu-id="117b2-116">La valeur **false** indique que la demande d’approbation a été décidée.</span><span class="sxs-lookup"><span data-stu-id="117b2-116">A value of **false** indicates that the approval request has been decided.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="117b2-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="117b2-117">Remarks</span></span>

<span data-ttu-id="117b2-118">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="117b2-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="117b2-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="117b2-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="117b2-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="117b2-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="117b2-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="117b2-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="117b2-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="117b2-122">Schema Name</span></span>  <br/> |<span data-ttu-id="117b2-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="117b2-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="117b2-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="117b2-124">Validation File</span></span>  <br/> |<span data-ttu-id="117b2-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="117b2-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="117b2-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="117b2-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="117b2-127">True</span><span class="sxs-lookup"><span data-stu-id="117b2-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="117b2-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="117b2-128">See also</span></span>



[<span data-ttu-id="117b2-129">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="117b2-129">ApprovalRequestData</span></span>](approvalrequestdata.md)


- [<span data-ttu-id="117b2-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="117b2-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

