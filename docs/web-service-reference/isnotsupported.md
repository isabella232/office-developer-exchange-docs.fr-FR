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
description: L’élément IsNotSupported indique si la règle ne peut pas être modifiée à l’aide des API avec code managé.
ms.openlocfilehash: e2d0c506209978fd5e8702e0de6cddf2e9c4b7fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465834"
---
# <a name="isnotsupported"></a><span data-ttu-id="158eb-103">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="158eb-103">IsNotSupported</span></span>

<span data-ttu-id="158eb-104">L’élément **IsNotSupported** indique si la règle ne peut pas être modifiée à l’aide des API avec code managé.</span><span class="sxs-lookup"><span data-stu-id="158eb-104">The **IsNotSupported** element indicates whether the rule cannot be modified by using the managed code APIs.</span></span> 
  
```XML
<IsNotSupported/>
```

 <span data-ttu-id="158eb-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="158eb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="158eb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="158eb-106">Attributes and elements</span></span>

<span data-ttu-id="158eb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="158eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="158eb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="158eb-108">Attributes</span></span>

<span data-ttu-id="158eb-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="158eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="158eb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="158eb-110">Child elements</span></span>

<span data-ttu-id="158eb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="158eb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="158eb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="158eb-112">Parent elements</span></span>

|<span data-ttu-id="158eb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="158eb-113">**Element**</span></span>|<span data-ttu-id="158eb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="158eb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="158eb-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="158eb-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="158eb-116">Représente une règle dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="158eb-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="158eb-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="158eb-117">Text value</span></span>

<span data-ttu-id="158eb-118">Une valeur de texte **true** indique que la règle ne peut pas être modifiée à l’aide des API avec code managé.</span><span class="sxs-lookup"><span data-stu-id="158eb-118">A text value of **true** indicates that the rule cannot be modified by using the managed code APIs.</span></span> <span data-ttu-id="158eb-119">La valeur **false** indique que la règle peut être modifiée à l’aide des API avec code managé.</span><span class="sxs-lookup"><span data-stu-id="158eb-119">A value of **false** indicates that the rule can be modified by using the managed code APIs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="158eb-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="158eb-120">Remarks</span></span>

<span data-ttu-id="158eb-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="158eb-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="158eb-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="158eb-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="158eb-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="158eb-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="158eb-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="158eb-124">Schema Name</span></span>  <br/> |<span data-ttu-id="158eb-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="158eb-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="158eb-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="158eb-126">Validation File</span></span>  <br/> |<span data-ttu-id="158eb-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="158eb-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="158eb-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="158eb-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="158eb-129">True</span><span class="sxs-lookup"><span data-stu-id="158eb-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="158eb-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="158eb-130">See also</span></span>



- [<span data-ttu-id="158eb-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="158eb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

