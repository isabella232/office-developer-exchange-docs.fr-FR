---
title: Priority
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Priority
api_type:
- schema
ms.assetid: e1adb8b9-e3d5-469a-b188-822733d2503e
description: L’élément de priorité indique l’ordre dans lequel une règle doit être exécutée.
ms.openlocfilehash: 49e9bda063d8766ff49c8a2e9574c986bcfdbeb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19828888"
---
# <a name="priority"></a><span data-ttu-id="98d01-103">Priority</span><span class="sxs-lookup"><span data-stu-id="98d01-103">Priority</span></span>

<span data-ttu-id="98d01-104">L’élément de **priorité** indique l’ordre dans lequel une règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="98d01-104">The **Priority** element indicates the order in which a rule is to be run.</span></span> 
  
```XML
<Priority/>
```

 <span data-ttu-id="98d01-105">**int**</span><span class="sxs-lookup"><span data-stu-id="98d01-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98d01-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="98d01-106">Attributes and elements</span></span>

<span data-ttu-id="98d01-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="98d01-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98d01-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="98d01-108">Attributes</span></span>

<span data-ttu-id="98d01-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="98d01-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98d01-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="98d01-110">Child elements</span></span>

<span data-ttu-id="98d01-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="98d01-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98d01-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="98d01-112">Parent elements</span></span>

|<span data-ttu-id="98d01-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="98d01-113">**Element**</span></span>|<span data-ttu-id="98d01-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="98d01-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98d01-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="98d01-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="98d01-116">Représente une règle de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="98d01-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98d01-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="98d01-117">Text value</span></span>

<span data-ttu-id="98d01-118">La valeur de texte de l’élément **dont la priorité** est un entier qui indique l’ordre d’exécution dans lequel une règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="98d01-118">The text value for the **Priority** element is an integer that indicates the execution order in which a rule should be run.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="98d01-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="98d01-119">Remarks</span></span>

<span data-ttu-id="98d01-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="98d01-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98d01-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="98d01-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98d01-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="98d01-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="98d01-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="98d01-123">Schema Name</span></span>  <br/> |<span data-ttu-id="98d01-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="98d01-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="98d01-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="98d01-125">Validation File</span></span>  <br/> |<span data-ttu-id="98d01-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="98d01-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="98d01-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="98d01-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="98d01-128">False</span><span class="sxs-lookup"><span data-stu-id="98d01-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98d01-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="98d01-129">See also</span></span>



- [<span data-ttu-id="98d01-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="98d01-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

