---
title: Date d’échéance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DueDate
api_type:
- schema
ms.assetid: dd9b6c43-a512-4b3b-a071-4abde02ed55f
description: L’élément DueDate représente la date d’échéance d’un élément.
ms.openlocfilehash: b88bb5c64ee48e02b1600c6865ce650e7bcdaa3b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463558"
---
# <a name="duedate"></a><span data-ttu-id="06f30-103">Date d’échéance</span><span class="sxs-lookup"><span data-stu-id="06f30-103">DueDate</span></span>

<span data-ttu-id="06f30-104">L’élément **DueDate** représente la date d’échéance d’un élément.</span><span class="sxs-lookup"><span data-stu-id="06f30-104">The **DueDate** element represents the date an item is due.</span></span> 
  
```xml
<DueDate/>
```

 <span data-ttu-id="06f30-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="06f30-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06f30-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="06f30-106">Attributes and elements</span></span>

<span data-ttu-id="06f30-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="06f30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06f30-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="06f30-108">Attributes</span></span>

<span data-ttu-id="06f30-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="06f30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06f30-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="06f30-110">Child elements</span></span>

<span data-ttu-id="06f30-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="06f30-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="06f30-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="06f30-112">Parent elements</span></span>

|<span data-ttu-id="06f30-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="06f30-113">**Element**</span></span>|<span data-ttu-id="06f30-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="06f30-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06f30-115">Tâche</span><span class="sxs-lookup"><span data-stu-id="06f30-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="06f30-116">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="06f30-116">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="06f30-117">Indicateur</span><span class="sxs-lookup"><span data-stu-id="06f30-117">Flag</span></span>](flag.md) <br/> |<span data-ttu-id="06f30-118">Spécifie un indicateur sur un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="06f30-118">Specifies a flag on a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06f30-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="06f30-119">Text value</span></span>

<span data-ttu-id="06f30-120">Une valeur de texte qui représente la date et l’heure est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="06f30-120">A text value that represents the date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06f30-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="06f30-121">Remarks</span></span>

<span data-ttu-id="06f30-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="06f30-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06f30-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="06f30-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06f30-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="06f30-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="06f30-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="06f30-125">Schema name</span></span>  <br/> |<span data-ttu-id="06f30-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="06f30-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="06f30-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="06f30-127">Validation file</span></span>  <br/> |<span data-ttu-id="06f30-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="06f30-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="06f30-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="06f30-129">Can be empty</span></span>  <br/> |<span data-ttu-id="06f30-130">False</span><span class="sxs-lookup"><span data-stu-id="06f30-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06f30-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="06f30-131">See also</span></span>

- [<span data-ttu-id="06f30-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="06f30-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

