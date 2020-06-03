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
description: L’élément Priority indique l’ordre dans lequel une règle doit être exécutée.
ms.openlocfilehash: a5a894bba583618dd04430fc89f125c8920b0202
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462401"
---
# <a name="priority"></a><span data-ttu-id="36dc1-103">Priority</span><span class="sxs-lookup"><span data-stu-id="36dc1-103">Priority</span></span>

<span data-ttu-id="36dc1-104">L’élément **Priority** indique l’ordre dans lequel une règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="36dc1-104">The **Priority** element indicates the order in which a rule is to be run.</span></span> 
  
```XML
<Priority/>
```

 <span data-ttu-id="36dc1-105">**int**</span><span class="sxs-lookup"><span data-stu-id="36dc1-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36dc1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="36dc1-106">Attributes and elements</span></span>

<span data-ttu-id="36dc1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="36dc1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36dc1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="36dc1-108">Attributes</span></span>

<span data-ttu-id="36dc1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="36dc1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36dc1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="36dc1-110">Child elements</span></span>

<span data-ttu-id="36dc1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="36dc1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36dc1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="36dc1-112">Parent elements</span></span>

|<span data-ttu-id="36dc1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="36dc1-113">**Element**</span></span>|<span data-ttu-id="36dc1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="36dc1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36dc1-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="36dc1-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="36dc1-116">Représente une règle dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="36dc1-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36dc1-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="36dc1-117">Text value</span></span>

<span data-ttu-id="36dc1-118">La valeur de texte pour l’élément **Priority** est un entier qui indique l’ordre d’exécution dans lequel une règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="36dc1-118">The text value for the **Priority** element is an integer that indicates the execution order in which a rule should be run.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="36dc1-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="36dc1-119">Remarks</span></span>

<span data-ttu-id="36dc1-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="36dc1-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36dc1-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="36dc1-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36dc1-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="36dc1-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="36dc1-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="36dc1-123">Schema Name</span></span>  <br/> |<span data-ttu-id="36dc1-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="36dc1-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="36dc1-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="36dc1-125">Validation File</span></span>  <br/> |<span data-ttu-id="36dc1-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="36dc1-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="36dc1-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="36dc1-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="36dc1-128">False</span><span class="sxs-lookup"><span data-stu-id="36dc1-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36dc1-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="36dc1-129">See also</span></span>



- [<span data-ttu-id="36dc1-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="36dc1-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

