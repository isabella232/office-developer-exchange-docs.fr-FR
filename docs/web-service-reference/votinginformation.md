---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: L’élément VotingInformation spécifie les informations de votantes whereApproveandRejectare de message de demande d’approbation message vote et les options de votantes.
ms.openlocfilehash: f11c25bb1f3a3c4781cfa6c51e11ff87af40c7f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839014"
---
# <a name="votinginformation"></a><span data-ttu-id="e4b98-103">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="e4b98-103">VotingInformation</span></span>

<span data-ttu-id="e4b98-104">L’élément **VotingInformation** spécifie les informations de votantes à un message de vote et le message de demande d’approbation où « Approuver » et « Refuser » est les options de votantes.</span><span class="sxs-lookup"><span data-stu-id="e4b98-104">The **VotingInformation** element specifies voting information on a voting message and approval request message where "Approve" and "Reject" are the voting options.</span></span> 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 <span data-ttu-id="e4b98-105">**VotingInformationType**</span><span class="sxs-lookup"><span data-stu-id="e4b98-105">**VotingInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4b98-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e4b98-106">Attributes and elements</span></span>

<span data-ttu-id="e4b98-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e4b98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4b98-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e4b98-108">Attributes</span></span>

<span data-ttu-id="e4b98-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e4b98-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4b98-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e4b98-110">Child elements</span></span>

<span data-ttu-id="e4b98-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span><span class="sxs-lookup"><span data-stu-id="e4b98-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4b98-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e4b98-112">Parent elements</span></span>

[<span data-ttu-id="e4b98-113">Message</span><span class="sxs-lookup"><span data-stu-id="e4b98-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="e4b98-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="e4b98-114">Remarks</span></span>

<span data-ttu-id="e4b98-115">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e4b98-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="e4b98-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4b98-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4b98-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e4b98-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4b98-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e4b98-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4b98-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e4b98-119">Schema Name</span></span>  <br/> |<span data-ttu-id="e4b98-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e4b98-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4b98-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e4b98-121">Validation File</span></span>  <br/> |<span data-ttu-id="e4b98-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e4b98-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4b98-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e4b98-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4b98-124">True</span><span class="sxs-lookup"><span data-stu-id="e4b98-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4b98-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e4b98-125">See also</span></span>



[<span data-ttu-id="e4b98-126">Message</span><span class="sxs-lookup"><span data-stu-id="e4b98-126">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="e4b98-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e4b98-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

