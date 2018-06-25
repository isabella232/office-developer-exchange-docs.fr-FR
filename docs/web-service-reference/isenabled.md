---
title: IsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEnabled
api_type:
- schema
ms.assetid: c7e3035e-a4ef-4c11-8cb0-214790a554ff
description: L’élément IsEnabled indique si la règle est activée.
ms.openlocfilehash: d0f0a77ec1ec952ac1cd9d9ad686ccfcb8f70c42
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828000"
---
# <a name="isenabled"></a><span data-ttu-id="919c1-103">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="919c1-103">IsEnabled</span></span>

<span data-ttu-id="919c1-104">L’élément **IsEnabled** indique si la règle est activée.</span><span class="sxs-lookup"><span data-stu-id="919c1-104">The **IsEnabled** element indicates whether the rule is enabled.</span></span> 
  
```XML
<IsEnabled/>
```

 <span data-ttu-id="919c1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="919c1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="919c1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="919c1-106">Attributes and elements</span></span>

<span data-ttu-id="919c1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="919c1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="919c1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="919c1-108">Attributes</span></span>

<span data-ttu-id="919c1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="919c1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="919c1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="919c1-110">Child elements</span></span>

<span data-ttu-id="919c1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="919c1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="919c1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="919c1-112">Parent elements</span></span>

|<span data-ttu-id="919c1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="919c1-113">**Element**</span></span>|<span data-ttu-id="919c1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="919c1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="919c1-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="919c1-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="919c1-116">Représente une règle de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="919c1-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="919c1-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="919c1-117">Text value</span></span>

<span data-ttu-id="919c1-118">Une valeur de texte de **la valeur true** indique que la règle est activée et peut être exécutée.</span><span class="sxs-lookup"><span data-stu-id="919c1-118">A text value of **true** indicates that the rule is enabled and can be executed.</span></span> <span data-ttu-id="919c1-119">La valeur **false** indique que la règle ne peut pas être exécutée.</span><span class="sxs-lookup"><span data-stu-id="919c1-119">A value of **false** indicates that the rule cannot be executed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="919c1-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="919c1-120">Remarks</span></span>

<span data-ttu-id="919c1-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="919c1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="919c1-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="919c1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="919c1-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="919c1-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="919c1-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="919c1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="919c1-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="919c1-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="919c1-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="919c1-126">Validation File</span></span>  <br/> |<span data-ttu-id="919c1-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="919c1-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="919c1-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="919c1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="919c1-129">True</span><span class="sxs-lookup"><span data-stu-id="919c1-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="919c1-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="919c1-130">See also</span></span>



- [<span data-ttu-id="919c1-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="919c1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

