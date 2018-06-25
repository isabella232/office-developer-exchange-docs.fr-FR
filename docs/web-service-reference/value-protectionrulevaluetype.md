---
title: Valeur (ProtectionRuleValueType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: b039bd6e-2198-47cf-9c78-a5e8b9d51c98
description: L’élément de valeur identifie un seul service destinataire ou l’expéditeur.
ms.openlocfilehash: 6173f94dcfb83eafd62e35f185a5e8c669d50f6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838999"
---
# <a name="value-protectionrulevaluetype"></a><span data-ttu-id="2ebed-103">Valeur (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="2ebed-103">Value (ProtectionRuleValueType)</span></span>

<span data-ttu-id="2ebed-104">L’élément de **valeur** identifie un seul service destinataire ou l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="2ebed-104">The **Value** element identifies a single recipient or sender department.</span></span> 
  
```XML
<Value/>
```

<span data-ttu-id="2ebed-105">**ProtectionRuleValueType**</span><span class="sxs-lookup"><span data-stu-id="2ebed-105">**ProtectionRuleValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2ebed-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ebed-106">Attributes and elements</span></span>

<span data-ttu-id="2ebed-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ebed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ebed-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ebed-108">Attributes</span></span>

<span data-ttu-id="2ebed-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ebed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ebed-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ebed-110">Child elements</span></span>

<span data-ttu-id="2ebed-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ebed-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ebed-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ebed-112">Parent elements</span></span>

|<span data-ttu-id="2ebed-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ebed-113">**Element**</span></span>|<span data-ttu-id="2ebed-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ebed-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ebed-115">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="2ebed-115">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="2ebed-116">Spécifie que n’importe quel destinataire du message électronique correspond à un des destinataires spécifiées dans les **valeur** des éléments enfants.</span><span class="sxs-lookup"><span data-stu-id="2ebed-116">Specifies that any recipient of the email message matches any of the specified recipients in the child **Value** elements.</span></span>  <br/> |
|[<span data-ttu-id="2ebed-117">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="2ebed-117">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="2ebed-118">Spécifie que le service de l’expéditeur correspond à l’un des services spécifiés dans les **valeur** des éléments enfants.</span><span class="sxs-lookup"><span data-stu-id="2ebed-118">Specifies that the department of the sender matches any of the specified departments in the child **Value** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ebed-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2ebed-119">Text value</span></span>

<span data-ttu-id="2ebed-120">Cet élément doit contenir une valeur de chaîne vide.</span><span class="sxs-lookup"><span data-stu-id="2ebed-120">This element must contain a nonempty string value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2ebed-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="2ebed-121">Remarks</span></span>

<span data-ttu-id="2ebed-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ebed-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ebed-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ebed-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ebed-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ebed-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ebed-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ebed-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2ebed-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2ebed-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ebed-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2ebed-127">Validation File</span></span>  <br/> |<span data-ttu-id="2ebed-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2ebed-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ebed-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ebed-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ebed-130">False</span><span class="sxs-lookup"><span data-stu-id="2ebed-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ebed-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2ebed-131">See also</span></span>

- [<span data-ttu-id="2ebed-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2ebed-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

