---
title: IsInError
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInError
api_type:
- schema
ms.assetid: f56e6c31-a566-4761-8755-d90ffe6fe790
description: L’élément IsInError indique si la règle est une condition d’erreur.
ms.openlocfilehash: 9f77bbe11106174d0e82c5257e08c3728d67c60c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828033"
---
# <a name="isinerror"></a><span data-ttu-id="9893f-103">IsInError</span><span class="sxs-lookup"><span data-stu-id="9893f-103">IsInError</span></span>

<span data-ttu-id="9893f-104">L’élément **IsInError** indique si la règle est une condition d’erreur.</span><span class="sxs-lookup"><span data-stu-id="9893f-104">The **IsInError** element indicates whether the rule is in an error condition.</span></span> 
  
```XML
<IsInError/>
```

 <span data-ttu-id="9893f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9893f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9893f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9893f-106">Attributes and elements</span></span>

<span data-ttu-id="9893f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9893f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9893f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9893f-108">Attributes</span></span>

<span data-ttu-id="9893f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9893f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9893f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9893f-110">Child elements</span></span>

<span data-ttu-id="9893f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9893f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9893f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9893f-112">Parent elements</span></span>

|<span data-ttu-id="9893f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9893f-113">**Element**</span></span>|<span data-ttu-id="9893f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9893f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9893f-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="9893f-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="9893f-116">Représente une règle de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9893f-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9893f-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9893f-117">Text value</span></span>

<span data-ttu-id="9893f-118">Une valeur de texte de **la valeur true** indique que la règle est une condition d’erreur.</span><span class="sxs-lookup"><span data-stu-id="9893f-118">A text value of **true** indicates that the rule is in an error condition.</span></span> <span data-ttu-id="9893f-119">La valeur **false** indique que la règle n’est pas une condition d’erreur.</span><span class="sxs-lookup"><span data-stu-id="9893f-119">A value of **false** indicates that the rule is not in an error condition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9893f-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="9893f-120">Remarks</span></span>

<span data-ttu-id="9893f-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9893f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9893f-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9893f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9893f-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9893f-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9893f-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9893f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9893f-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9893f-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9893f-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9893f-126">Validation File</span></span>  <br/> |<span data-ttu-id="9893f-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9893f-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9893f-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9893f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="9893f-129">True</span><span class="sxs-lookup"><span data-stu-id="9893f-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9893f-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9893f-130">See also</span></span>



- [<span data-ttu-id="9893f-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9893f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

