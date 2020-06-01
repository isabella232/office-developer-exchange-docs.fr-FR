---
title: InboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InboxRules
api_type:
- schema
ms.assetid: 7bb9896c-bd12-49ae-842a-a10b5f9a2ef6
description: L'élément InboxRules représente un tableau de règles de boîte aux lettres de l'utilisateur.
ms.openlocfilehash: a3107c3c317a912d0bd3e60d03da4168f2f3a0a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458270"
---
# <a name="inboxrules"></a><span data-ttu-id="0d8ae-103">InboxRules</span><span class="sxs-lookup"><span data-stu-id="0d8ae-103">InboxRules</span></span>

<span data-ttu-id="0d8ae-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **InboxRules** représente un tableau de règles de boîte aux lettres de l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="0d8ae-104">The **InboxRules** element represents an array of rules in the user's mailbox.</span></span> 
  
[<span data-ttu-id="0d8ae-105">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="0d8ae-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="0d8ae-106">InboxRules</span><span class="sxs-lookup"><span data-stu-id="0d8ae-106">InboxRules</span></span>](inboxrules.md)
  
```XML
<InboxRules>
   <Rule/>
</InboxRules>
```

 <span data-ttu-id="0d8ae-107">**ArrayOfRulesType**</span><span class="sxs-lookup"><span data-stu-id="0d8ae-107">**ArrayOfRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d8ae-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0d8ae-108">Attributes and elements</span></span>

<span data-ttu-id="0d8ae-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0d8ae-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d8ae-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="0d8ae-110">Attributes</span></span>

<span data-ttu-id="0d8ae-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0d8ae-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d8ae-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0d8ae-112">Child elements</span></span>

|<span data-ttu-id="0d8ae-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0d8ae-113">**Element**</span></span>|<span data-ttu-id="0d8ae-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0d8ae-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d8ae-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="0d8ae-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="0d8ae-116">Contient une règle unique et représente une règle de boîte aux lettres de l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="0d8ae-116">Contains a single rule and represents a rule in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0d8ae-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0d8ae-117">Parent elements</span></span>

|<span data-ttu-id="0d8ae-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0d8ae-118">**Element**</span></span>|<span data-ttu-id="0d8ae-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="0d8ae-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d8ae-120">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="0d8ae-120">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="0d8ae-121">Définit une réponse à une demande de [Opération de GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0d8ae-121">Defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0d8ae-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0d8ae-122">Text value</span></span>

<span data-ttu-id="0d8ae-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0d8ae-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0d8ae-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="0d8ae-124">Remarks</span></span>

<span data-ttu-id="0d8ae-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d8ae-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d8ae-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0d8ae-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d8ae-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0d8ae-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0d8ae-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0d8ae-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0d8ae-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0d8ae-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0d8ae-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0d8ae-130">Validation File</span></span>  <br/> |<span data-ttu-id="0d8ae-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0d8ae-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0d8ae-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0d8ae-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d8ae-133">True</span><span class="sxs-lookup"><span data-stu-id="0d8ae-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d8ae-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0d8ae-134">See also</span></span>



[<span data-ttu-id="0d8ae-135">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="0d8ae-135">GetInboxRules</span></span>](getinboxrules.md)
  
[<span data-ttu-id="0d8ae-136">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="0d8ae-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)


- [<span data-ttu-id="0d8ae-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0d8ae-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

