---
title: Destinataireest
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
description: L’élément Recipient spécifie que tout destinataire du message électronique correspond à l’un des destinataires spécifiés dans les éléments de valeur enfant (ProtectionRuleValueType).
ms.openlocfilehash: 8f27c4484ce310c62f9bab0e6ffeea2bfac1d3ef
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463880"
---
# <a name="recipientis"></a><span data-ttu-id="de3e6-103">Destinataireest</span><span class="sxs-lookup"><span data-stu-id="de3e6-103">RecipientIs</span></span>

<span data-ttu-id="de3e6-104">L’élément **Recipient** spécifie que tout destinataire du message électronique correspond à l’un des destinataires spécifiés dans les éléments de [valeur enfant (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="de3e6-104">The **RecipientIs** element specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 <span data-ttu-id="de3e6-105">**ProtectionRuleRecipientIsType**</span><span class="sxs-lookup"><span data-stu-id="de3e6-105">**ProtectionRuleRecipientIsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de3e6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="de3e6-106">Attributes and elements</span></span>

<span data-ttu-id="de3e6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="de3e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de3e6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="de3e6-108">Attributes</span></span>

<span data-ttu-id="de3e6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="de3e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de3e6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="de3e6-110">Child elements</span></span>

|<span data-ttu-id="de3e6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="de3e6-111">**Element**</span></span>|<span data-ttu-id="de3e6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="de3e6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de3e6-113">Valeur (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="de3e6-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="de3e6-114">Identifie un destinataire.</span><span class="sxs-lookup"><span data-stu-id="de3e6-114">Identifies a recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="de3e6-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="de3e6-115">Parent elements</span></span>

|<span data-ttu-id="de3e6-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="de3e6-116">**Element**</span></span>|<span data-ttu-id="de3e6-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="de3e6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de3e6-118">Condition</span><span class="sxs-lookup"><span data-stu-id="de3e6-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="de3e6-119">Identifie la condition qui doit être remplie pour que la partie action de la règle soit exécutée.</span><span class="sxs-lookup"><span data-stu-id="de3e6-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="de3e6-120">Et (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="de3e6-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="de3e6-121">Indique que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="de3e6-121">Indicates that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="de3e6-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="de3e6-122">Remarks</span></span>

<span data-ttu-id="de3e6-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="de3e6-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de3e6-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="de3e6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de3e6-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="de3e6-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de3e6-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="de3e6-126">Schema Name</span></span>  <br/> |<span data-ttu-id="de3e6-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="de3e6-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="de3e6-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="de3e6-128">Validation File</span></span>  <br/> |<span data-ttu-id="de3e6-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="de3e6-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de3e6-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="de3e6-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="de3e6-131">False</span><span class="sxs-lookup"><span data-stu-id="de3e6-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de3e6-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="de3e6-132">See also</span></span>



- [<span data-ttu-id="de3e6-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="de3e6-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

