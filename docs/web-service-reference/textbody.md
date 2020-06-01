---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: L’élément TextBody spécifie le corps du texte.
ms.openlocfilehash: c0002785fb990a251267218f7a5f232e521db41a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459482"
---
# <a name="textbody"></a><span data-ttu-id="a4b66-103">TextBody</span><span class="sxs-lookup"><span data-stu-id="a4b66-103">TextBody</span></span>

<span data-ttu-id="a4b66-104">L’élément **TextBody** spécifie le corps du texte.</span><span class="sxs-lookup"><span data-stu-id="a4b66-104">The **TextBody** element specifies the text body.</span></span> 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 <span data-ttu-id="a4b66-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="a4b66-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4b66-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a4b66-106">Attributes and elements</span></span>

<span data-ttu-id="a4b66-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a4b66-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4b66-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a4b66-108">Attributes</span></span>

|<span data-ttu-id="a4b66-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a4b66-109">**Attribute**</span></span>|<span data-ttu-id="a4b66-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="a4b66-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a4b66-111">BodyTypeType</span><span class="sxs-lookup"><span data-stu-id="a4b66-111">BodyTypeType</span></span>  <br/> |<span data-ttu-id="a4b66-112">Indique le type de corps.</span><span class="sxs-lookup"><span data-stu-id="a4b66-112">Indicates the body type.</span></span> <span data-ttu-id="a4b66-113">La valeur de **Text** pour l’attribut **BodyTypeType** indique que le corps est en texte brut.</span><span class="sxs-lookup"><span data-stu-id="a4b66-113">The value of **Text** for the **BodyTypeType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="a4b66-114">La valeur de **HTML** pour l’attribut **BodyTypeType** indique que le corps est au format html.</span><span class="sxs-lookup"><span data-stu-id="a4b66-114">The value of **HTML** for the **BodyTypeType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="a4b66-115">L’attribut **BodyTypeType** est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="a4b66-115">The **BodyTypeType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="a4b66-116">IsTruncated</span><span class="sxs-lookup"><span data-stu-id="a4b66-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="a4b66-117">Indique que le contenu du corps a été tronqué.</span><span class="sxs-lookup"><span data-stu-id="a4b66-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="a4b66-118">Une valeur de texte **false** pour l’attribut **IsTruncated** indique que le contenu du corps n’a pas été tronqué.</span><span class="sxs-lookup"><span data-stu-id="a4b66-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="a4b66-119">Le corps normalisé est tronqué si la longueur du corps du texte est supérieure à la valeur définie dans l’élément [MaximumBodySize](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="a4b66-119">The normalized body will be truncated if the text body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a4b66-120">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a4b66-120">Child elements</span></span>

<span data-ttu-id="a4b66-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a4b66-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4b66-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a4b66-122">Parent elements</span></span>

<span data-ttu-id="a4b66-123">[Élément](item.md)  |  [Contact](contact.md)  |  [Message](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tâche](task.md)</span><span class="sxs-lookup"><span data-stu-id="a4b66-123">[Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a4b66-124">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a4b66-124">Text value</span></span>

<span data-ttu-id="a4b66-125">La valeur de texte de l’élément **TextBody** est le corps de texte de l’élément.</span><span class="sxs-lookup"><span data-stu-id="a4b66-125">The text value of the **TextBody** element is the text body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a4b66-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="a4b66-126">Remarks</span></span>

<span data-ttu-id="a4b66-127">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a4b66-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a4b66-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a4b66-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4b66-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a4b66-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4b66-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a4b66-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a4b66-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a4b66-131">Schema name</span></span>  <br/> |<span data-ttu-id="a4b66-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a4b66-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="a4b66-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a4b66-133">Validation file</span></span>  <br/> |<span data-ttu-id="a4b66-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a4b66-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a4b66-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a4b66-135">Can be empty</span></span>  <br/> ||
   

