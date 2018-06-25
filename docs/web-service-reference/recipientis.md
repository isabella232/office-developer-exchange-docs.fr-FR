---
title: RecipientIs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientIs
api_type:
- schema
ms.assetid: 5d2fd7ce-6137-4b3c-a716-c0218dcc8a09
description: L’élément RecipientIs Spécifie que n’importe quel destinataire du message électronique correspond à un des destinataires spécifiés dans les éléments de valeur (ProtectionRuleValueType) enfants.
ms.openlocfilehash: b6d5c150cd874d1aced7f2d83ff36409e0738728
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828975"
---
# <a name="recipientis"></a><span data-ttu-id="85766-103">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="85766-103">RecipientIs</span></span>

<span data-ttu-id="85766-104">L’élément **RecipientIs** Spécifie que n’importe quel destinataire du message électronique correspond à un des destinataires spécifiés dans les éléments de [valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) enfants.</span><span class="sxs-lookup"><span data-stu-id="85766-104">The **RecipientIs** element specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 <span data-ttu-id="85766-105">**ProtectionRuleRecipientIsType**</span><span class="sxs-lookup"><span data-stu-id="85766-105">**ProtectionRuleRecipientIsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85766-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="85766-106">Attributes and elements</span></span>

<span data-ttu-id="85766-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="85766-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85766-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="85766-108">Attributes</span></span>

<span data-ttu-id="85766-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="85766-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85766-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="85766-110">Child elements</span></span>

|<span data-ttu-id="85766-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85766-111">**Element**</span></span>|<span data-ttu-id="85766-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="85766-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85766-113">Valeur (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="85766-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="85766-114">Identifie un destinataire.</span><span class="sxs-lookup"><span data-stu-id="85766-114">Identifies a recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85766-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="85766-115">Parent elements</span></span>

|<span data-ttu-id="85766-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85766-116">**Element**</span></span>|<span data-ttu-id="85766-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="85766-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85766-118">Condition</span><span class="sxs-lookup"><span data-stu-id="85766-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="85766-119">Identifie la condition qui doit être remplie pour la partie de l’action de la règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="85766-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="85766-120">Et (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="85766-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="85766-121">Indique que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="85766-121">Indicates that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="85766-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="85766-122">Remarks</span></span>

<span data-ttu-id="85766-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="85766-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85766-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="85766-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85766-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="85766-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85766-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="85766-126">Schema Name</span></span>  <br/> |<span data-ttu-id="85766-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="85766-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="85766-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="85766-128">Validation File</span></span>  <br/> |<span data-ttu-id="85766-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="85766-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85766-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="85766-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="85766-131">False</span><span class="sxs-lookup"><span data-stu-id="85766-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85766-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="85766-132">See also</span></span>



- [<span data-ttu-id="85766-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="85766-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

