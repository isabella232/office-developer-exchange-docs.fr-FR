---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: L’élément NormalizedBody spécifie une représentation HTML de la propriété Body d’un élément en tant que fragment qui peut être inséré dans un autre corps HTML.
ms.openlocfilehash: 07c2176d2c8a7473c06b7e42f8bcbbe6670581ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828548"
---
# <a name="normalizedbody"></a><span data-ttu-id="0f710-103">NormalizedBody</span><span class="sxs-lookup"><span data-stu-id="0f710-103">NormalizedBody</span></span>

<span data-ttu-id="0f710-104">L’élément **NormalizedBody** spécifie une représentation HTML de la propriété **Body** d’un élément en tant que fragment qui peut être inséré dans un autre corps HTML.</span><span class="sxs-lookup"><span data-stu-id="0f710-104">The **NormalizedBody** element specifies an HTML representation of the **Body** property of an item as a fragment that can be inserted into another HTML body.</span></span> 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 <span data-ttu-id="0f710-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="0f710-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f710-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0f710-106">Attributes and elements</span></span>

<span data-ttu-id="0f710-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0f710-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f710-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0f710-108">Attributes</span></span>

|<span data-ttu-id="0f710-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="0f710-109">**Attribute**</span></span>|<span data-ttu-id="0f710-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f710-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0f710-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="0f710-111">BodyType</span></span>  <br/> |<span data-ttu-id="0f710-112">Indique le type de corps.</span><span class="sxs-lookup"><span data-stu-id="0f710-112">Indicates the body type.</span></span> <span data-ttu-id="0f710-113">La valeur de **texte** pour l’attribut **BodyType** indique que le corps est au format texte brut.</span><span class="sxs-lookup"><span data-stu-id="0f710-113">The value of **Text** for the **BodyType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="0f710-114">La valeur de **code HTML** pour l’attribut **BodyType** indique que le corps est au format HTML.</span><span class="sxs-lookup"><span data-stu-id="0f710-114">The value of **HTML** for the **BodyType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="0f710-115">L’attribut **BodyType** est requis.</span><span class="sxs-lookup"><span data-stu-id="0f710-115">The **BodyType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="0f710-116">IsTruncated</span><span class="sxs-lookup"><span data-stu-id="0f710-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="0f710-117">Indique que le contenu du corps a été tronqué.</span><span class="sxs-lookup"><span data-stu-id="0f710-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="0f710-118">Texte la valeur **false** pour l’attribut **IsTruncated** indique que le contenu du corps n’a pas été tronqué.</span><span class="sxs-lookup"><span data-stu-id="0f710-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="0f710-119">Si la longueur de corps normalisée est supérieure à la valeur définie dans l’élément [MaximumBodySize](maximumbodysize.md) le corps normalisé sera tronqué.</span><span class="sxs-lookup"><span data-stu-id="0f710-119">The normalized body will be truncated if the normalized body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0f710-120">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0f710-120">Child elements</span></span>

<span data-ttu-id="0f710-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0f710-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0f710-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0f710-122">Parent elements</span></span>

<span data-ttu-id="0f710-123">[Élément](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [tâche](task.md) | [PostItem ](postitem.md)  |  [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="0f710-123">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0f710-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0f710-124">Text value</span></span>

<span data-ttu-id="0f710-125">La valeur de texte de l’élément **NormalizedBody** est le corps de l’élément normalisé.</span><span class="sxs-lookup"><span data-stu-id="0f710-125">The text value of the **NormalizedBody** element is the normalized body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0f710-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="0f710-126">Remarks</span></span>

<span data-ttu-id="0f710-127">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0f710-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0f710-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f710-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f710-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0f710-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f710-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0f710-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f710-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0f710-131">Schema name</span></span>  <br/> |<span data-ttu-id="0f710-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0f710-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f710-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0f710-133">Validation file</span></span>  <br/> |<span data-ttu-id="0f710-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0f710-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f710-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0f710-135">Can be empty</span></span>  <br/> ||
   

