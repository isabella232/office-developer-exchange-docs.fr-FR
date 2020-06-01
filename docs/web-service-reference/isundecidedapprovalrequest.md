---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: L’élément IsUndecidedApprovalRequest spécifie si un message de demande d’approbation a été traité.
ms.openlocfilehash: 0949cf64b8583c4b3fa5a1700475f01cc480f69f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458172"
---
# <a name="isundecidedapprovalrequest"></a><span data-ttu-id="023f7-103">IsUndecidedApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="023f7-103">IsUndecidedApprovalRequest</span></span>

<span data-ttu-id="023f7-104">L’élément **IsUndecidedApprovalRequest** spécifie si un message de demande d’approbation a été traité.</span><span class="sxs-lookup"><span data-stu-id="023f7-104">The **IsUndecidedApprovalRequest** element specifies whether an approval request message has been acted on.</span></span> 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 <span data-ttu-id="023f7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="023f7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="023f7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="023f7-106">Attributes and elements</span></span>

<span data-ttu-id="023f7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="023f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="023f7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="023f7-108">Attributes</span></span>

<span data-ttu-id="023f7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="023f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="023f7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="023f7-110">Child elements</span></span>

<span data-ttu-id="023f7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="023f7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="023f7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="023f7-112">Parent elements</span></span>

[<span data-ttu-id="023f7-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="023f7-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="023f7-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="023f7-114">Text value</span></span>

<span data-ttu-id="023f7-115">La valeur de texte de l’élément **IsUndecidedApprovalRequest** est **true** si aucun message de demande d’approbation n’a été traité.</span><span class="sxs-lookup"><span data-stu-id="023f7-115">The text value of the **IsUndecidedApprovalRequest** element is **true** if an approval request message has not been acted on.</span></span> <span data-ttu-id="023f7-116">La valeur **false** indique que la demande d’approbation a été décidée.</span><span class="sxs-lookup"><span data-stu-id="023f7-116">A value of **false** indicates that the approval request has been decided.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="023f7-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="023f7-117">Remarks</span></span>

<span data-ttu-id="023f7-118">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="023f7-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="023f7-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="023f7-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="023f7-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="023f7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="023f7-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="023f7-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="023f7-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="023f7-122">Schema Name</span></span>  <br/> |<span data-ttu-id="023f7-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="023f7-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="023f7-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="023f7-124">Validation File</span></span>  <br/> |<span data-ttu-id="023f7-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="023f7-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="023f7-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="023f7-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="023f7-127">True</span><span class="sxs-lookup"><span data-stu-id="023f7-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="023f7-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="023f7-128">See also</span></span>



[<span data-ttu-id="023f7-129">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="023f7-129">ApprovalRequestData</span></span>](approvalrequestdata.md)


- [<span data-ttu-id="023f7-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="023f7-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

