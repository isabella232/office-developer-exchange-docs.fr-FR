---
title: IsApprovalRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsApprovalRequest
api_type:
- schema
ms.assetid: 293ed01b-f6a4-4459-819c-933bbfaa2dd7
description: L’élément IsApprovalRequest indique si les messages entrants doivent être des demandes d’approbation afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 08ea36820b2680bb2c7e5695eb2dd481154c05eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530013"
---
# <a name="isapprovalrequest"></a><span data-ttu-id="519c7-103">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="519c7-103">IsApprovalRequest</span></span>

<span data-ttu-id="519c7-104">L’élément **IsApprovalRequest** indique si les messages entrants doivent être des demandes d’approbation afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="519c7-104">The **IsApprovalRequest** element indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span> 
  
```XML
<IsApprovalRequest/>
```

 <span data-ttu-id="519c7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="519c7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="519c7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="519c7-106">Attributes and elements</span></span>

<span data-ttu-id="519c7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="519c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="519c7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="519c7-108">Attributes</span></span>

<span data-ttu-id="519c7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="519c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="519c7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="519c7-110">Child elements</span></span>

<span data-ttu-id="519c7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="519c7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="519c7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="519c7-112">Parent elements</span></span>

|<span data-ttu-id="519c7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="519c7-113">**Element**</span></span>|<span data-ttu-id="519c7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="519c7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="519c7-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="519c7-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="519c7-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="519c7-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="519c7-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="519c7-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="519c7-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="519c7-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="519c7-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="519c7-119">Text value</span></span>

<span data-ttu-id="519c7-120">Une valeur de texte **true** indique que le message doit être une demande d’approbation afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="519c7-120">A text value of **true** indicates that the message must be an approval request in order for the condition or exception to apply.</span></span> <span data-ttu-id="519c7-121">La valeur **false** indique que le message ne doit pas être une demande d’approbation afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="519c7-121">A value of **false** indicates that the message must not be an approval request in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="519c7-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="519c7-122">Remarks</span></span>

<span data-ttu-id="519c7-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="519c7-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="519c7-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="519c7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="519c7-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="519c7-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="519c7-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="519c7-126">Schema Name</span></span>  <br/> |<span data-ttu-id="519c7-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="519c7-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="519c7-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="519c7-128">Validation File</span></span>  <br/> |<span data-ttu-id="519c7-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="519c7-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="519c7-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="519c7-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="519c7-131">True</span><span class="sxs-lookup"><span data-stu-id="519c7-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="519c7-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="519c7-132">See also</span></span>



- [<span data-ttu-id="519c7-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="519c7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

