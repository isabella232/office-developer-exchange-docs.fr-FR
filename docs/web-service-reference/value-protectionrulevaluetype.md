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
description: L’élément Value identifie un service de destinataire ou d’expéditeur unique.
ms.openlocfilehash: 908ea451800abc343fb6e4d4a4ed98d57223bd23
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465239"
---
# <a name="value-protectionrulevaluetype"></a><span data-ttu-id="00c41-103">Valeur (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="00c41-103">Value (ProtectionRuleValueType)</span></span>

<span data-ttu-id="00c41-104">L’élément **value** identifie un service de destinataire ou d’expéditeur unique.</span><span class="sxs-lookup"><span data-stu-id="00c41-104">The **Value** element identifies a single recipient or sender department.</span></span> 
  
```XML
<Value/>
```

<span data-ttu-id="00c41-105">**ProtectionRuleValueType**</span><span class="sxs-lookup"><span data-stu-id="00c41-105">**ProtectionRuleValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="00c41-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00c41-106">Attributes and elements</span></span>

<span data-ttu-id="00c41-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00c41-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00c41-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="00c41-108">Attributes</span></span>

<span data-ttu-id="00c41-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="00c41-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00c41-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00c41-110">Child elements</span></span>

<span data-ttu-id="00c41-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="00c41-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="00c41-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00c41-112">Parent elements</span></span>

|<span data-ttu-id="00c41-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00c41-113">**Element**</span></span>|<span data-ttu-id="00c41-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="00c41-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00c41-115">Destinataireest</span><span class="sxs-lookup"><span data-stu-id="00c41-115">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="00c41-116">Spécifie que tout destinataire du message électronique correspond à l’un des destinataires spécifiés dans les éléments de **valeur** enfants.</span><span class="sxs-lookup"><span data-stu-id="00c41-116">Specifies that any recipient of the email message matches any of the specified recipients in the child **Value** elements.</span></span>  <br/> |
|[<span data-ttu-id="00c41-117">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="00c41-117">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="00c41-118">Spécifie que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de **valeur** enfants.</span><span class="sxs-lookup"><span data-stu-id="00c41-118">Specifies that the department of the sender matches any of the specified departments in the child **Value** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00c41-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="00c41-119">Text value</span></span>

<span data-ttu-id="00c41-120">Cet élément doit contenir une valeur de chaîne non vide.</span><span class="sxs-lookup"><span data-stu-id="00c41-120">This element must contain a nonempty string value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00c41-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="00c41-121">Remarks</span></span>

<span data-ttu-id="00c41-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="00c41-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00c41-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00c41-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00c41-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00c41-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00c41-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00c41-125">Schema Name</span></span>  <br/> |<span data-ttu-id="00c41-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="00c41-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="00c41-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="00c41-127">Validation File</span></span>  <br/> |<span data-ttu-id="00c41-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="00c41-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00c41-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00c41-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="00c41-130">False</span><span class="sxs-lookup"><span data-stu-id="00c41-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00c41-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00c41-131">See also</span></span>

- [<span data-ttu-id="00c41-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="00c41-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

