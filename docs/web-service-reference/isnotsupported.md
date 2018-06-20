---
title: IsNotSupported
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotSupported
api_type:
- schema
ms.assetid: 4db469ae-1515-47ea-9905-6aabf199febd
description: L’élément IsNotSupported indique si la règle ne peut pas être modifiée à l’aide de l’API de code managé.
ms.openlocfilehash: 2468d47dbfdcaf1a28ed1a4afb1e7ea60147d1dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828057"
---
# <a name="isnotsupported"></a><span data-ttu-id="10b2e-103">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="10b2e-103">IsNotSupported</span></span>

<span data-ttu-id="10b2e-104">L’élément **IsNotSupported** indique si la règle ne peut pas être modifiée à l’aide de l’API de code managé.</span><span class="sxs-lookup"><span data-stu-id="10b2e-104">The **IsNotSupported** element indicates whether the rule cannot be modified by using the managed code APIs.</span></span> 
  
```XML
<IsNotSupported/>
```

 <span data-ttu-id="10b2e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="10b2e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="10b2e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="10b2e-106">Attributes and elements</span></span>

<span data-ttu-id="10b2e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="10b2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10b2e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="10b2e-108">Attributes</span></span>

<span data-ttu-id="10b2e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="10b2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10b2e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="10b2e-110">Child elements</span></span>

<span data-ttu-id="10b2e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="10b2e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="10b2e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="10b2e-112">Parent elements</span></span>

|<span data-ttu-id="10b2e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="10b2e-113">**Element**</span></span>|<span data-ttu-id="10b2e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="10b2e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10b2e-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="10b2e-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="10b2e-116">Représente une règle de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="10b2e-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="10b2e-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="10b2e-117">Text value</span></span>

<span data-ttu-id="10b2e-118">Une valeur de texte de **la valeur true** indique que la règle ne peut pas être modifiée à l’aide de l’API de code managé.</span><span class="sxs-lookup"><span data-stu-id="10b2e-118">A text value of **true** indicates that the rule cannot be modified by using the managed code APIs.</span></span> <span data-ttu-id="10b2e-119">La valeur **false** indique que la règle peut être modifiée à l’aide de l’API de code managé.</span><span class="sxs-lookup"><span data-stu-id="10b2e-119">A value of **false** indicates that the rule can be modified by using the managed code APIs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="10b2e-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="10b2e-120">Remarks</span></span>

<span data-ttu-id="10b2e-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="10b2e-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10b2e-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="10b2e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10b2e-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="10b2e-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="10b2e-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="10b2e-124">Schema Name</span></span>  <br/> |<span data-ttu-id="10b2e-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="10b2e-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="10b2e-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="10b2e-126">Validation File</span></span>  <br/> |<span data-ttu-id="10b2e-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="10b2e-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="10b2e-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="10b2e-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="10b2e-129">True</span><span class="sxs-lookup"><span data-stu-id="10b2e-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10b2e-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="10b2e-130">See also</span></span>



- [<span data-ttu-id="10b2e-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="10b2e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
