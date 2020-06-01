---
title: EndDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDateTime
api_type:
- schema
ms.assetid: 54d14e47-a8f7-400b-a859-c7ea7ce4c6a4
description: L’élément EndDateTime spécifie la date et l’heure de fin d’une règle ou d’une recherche.
ms.openlocfilehash: 9556e4c1ef405ae66a71d19d99d9a71a61f54efc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460133"
---
# <a name="enddatetime"></a><span data-ttu-id="b3b3c-103">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="b3b3c-103">EndDateTime</span></span>

<span data-ttu-id="b3b3c-104">L’élément **EndDateTime** spécifie la date et l’heure de fin d’une règle ou d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="b3b3c-104">The **EndDateTime** element specifies the end date and time for a rule or a search.</span></span> 
  
```XML
<EndDateTime/>
```

 <span data-ttu-id="b3b3c-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="b3b3c-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3b3c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b3b3c-106">Attributes and elements</span></span>

<span data-ttu-id="b3b3c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b3b3c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3b3c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b3b3c-108">Attributes</span></span>

<span data-ttu-id="b3b3c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b3b3c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3b3c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b3b3c-110">Child elements</span></span>

<span data-ttu-id="b3b3c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b3b3c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b3b3c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b3b3c-112">Parent elements</span></span>

|<span data-ttu-id="b3b3c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b3b3c-113">**Element**</span></span>|<span data-ttu-id="b3b3c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b3b3c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3b3c-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b3b3c-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="b3b3c-116">Contient des critères pour les types de messages à rechercher.</span><span class="sxs-lookup"><span data-stu-id="b3b3c-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="b3b3c-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="b3b3c-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="b3b3c-118">Spécifie la plage de dates au cours de laquelle les messages entrants doivent avoir été reçus afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="b3b3c-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b3b3c-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="b3b3c-119">Text value</span></span>

<span data-ttu-id="b3b3c-120">Une valeur de texte qui représente une date/heure est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="b3b3c-120">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b3b3c-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="b3b3c-121">Remarks</span></span>

<span data-ttu-id="b3b3c-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3b3c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3b3c-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b3b3c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3b3c-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b3b3c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b3b3c-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b3b3c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b3b3c-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b3b3c-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b3b3c-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b3b3c-127">Validation File</span></span>  <br/> |<span data-ttu-id="b3b3c-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b3b3c-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b3b3c-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b3b3c-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="b3b3c-130">False</span><span class="sxs-lookup"><span data-stu-id="b3b3c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3b3c-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b3b3c-131">See also</span></span>



- [<span data-ttu-id="b3b3c-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b3b3c-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

