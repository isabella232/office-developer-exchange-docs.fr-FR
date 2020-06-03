---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: L’élément NormalizedBody spécifie une représentation HTML de la propriété Body d’un élément sous la forme d’un fragment qui peut être inséré dans un autre corps HTML.
ms.openlocfilehash: fb249794bccfeed198e7a3230ab53c66893dcf96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462667"
---
# <a name="normalizedbody"></a><span data-ttu-id="22843-103">NormalizedBody</span><span class="sxs-lookup"><span data-stu-id="22843-103">NormalizedBody</span></span>

<span data-ttu-id="22843-104">L’élément **NormalizedBody** spécifie une représentation HTML de la propriété **Body** d’un élément sous la forme d’un fragment qui peut être inséré dans un autre corps HTML.</span><span class="sxs-lookup"><span data-stu-id="22843-104">The **NormalizedBody** element specifies an HTML representation of the **Body** property of an item as a fragment that can be inserted into another HTML body.</span></span> 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 <span data-ttu-id="22843-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="22843-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22843-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22843-106">Attributes and elements</span></span>

<span data-ttu-id="22843-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22843-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22843-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="22843-108">Attributes</span></span>

|<span data-ttu-id="22843-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="22843-109">**Attribute**</span></span>|<span data-ttu-id="22843-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="22843-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="22843-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="22843-111">BodyType</span></span>  <br/> |<span data-ttu-id="22843-112">Indique le type de corps.</span><span class="sxs-lookup"><span data-stu-id="22843-112">Indicates the body type.</span></span> <span data-ttu-id="22843-113">La valeur de **Text** pour l’attribut **BodyType** indique que le corps est en texte brut.</span><span class="sxs-lookup"><span data-stu-id="22843-113">The value of **Text** for the **BodyType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="22843-114">La valeur de **HTML** pour l’attribut **BodyType** indique que le corps est au format html.</span><span class="sxs-lookup"><span data-stu-id="22843-114">The value of **HTML** for the **BodyType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="22843-115">L’attribut **BodyType** est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="22843-115">The **BodyType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="22843-116">IsTruncated</span><span class="sxs-lookup"><span data-stu-id="22843-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="22843-117">Indique que le contenu du corps a été tronqué.</span><span class="sxs-lookup"><span data-stu-id="22843-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="22843-118">Une valeur de texte **false** pour l’attribut **IsTruncated** indique que le contenu du corps n’a pas été tronqué.</span><span class="sxs-lookup"><span data-stu-id="22843-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="22843-119">Le corps normalisé est tronqué si la longueur de corps normalisé est supérieure à la valeur définie dans l’élément [MaximumBodySize](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="22843-119">The normalized body will be truncated if the normalized body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="22843-120">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22843-120">Child elements</span></span>

<span data-ttu-id="22843-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="22843-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="22843-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22843-122">Parent elements</span></span>

<span data-ttu-id="22843-123">[Élément](item.md)  |  [Message](message-ex15websvcsotherref.md)  |  [MeetingMessage](meetingmessage.md)  |  [Propriété meetingrequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [Tâche](task.md)  |  [PostItem](postitem.md)  |  [CalendarItem](calendaritem.md)  |  [Contact](contact.md)  |  [DistributionList](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="22843-123">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="22843-124">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="22843-124">Text value</span></span>

<span data-ttu-id="22843-125">La valeur de texte de l’élément **NormalizedBody** est le corps normalisé de l’élément.</span><span class="sxs-lookup"><span data-stu-id="22843-125">The text value of the **NormalizedBody** element is the normalized body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="22843-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="22843-126">Remarks</span></span>

<span data-ttu-id="22843-127">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="22843-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="22843-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="22843-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22843-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22843-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22843-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22843-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22843-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22843-131">Schema name</span></span>  <br/> |<span data-ttu-id="22843-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="22843-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="22843-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22843-133">Validation file</span></span>  <br/> |<span data-ttu-id="22843-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="22843-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="22843-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22843-135">Can be empty</span></span>  <br/> ||
   

