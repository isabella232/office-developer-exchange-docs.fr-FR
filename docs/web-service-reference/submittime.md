---
title: SubmitTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubmitTime
api_type:
- schema
ms.assetid: 97e4b71e-f45c-4bdb-80f9-805934916c0f
description: L’élément SubmitTime représente l’heure à laquelle le message a été envoyé au serveur.
ms.openlocfilehash: e4409d962988ee308e0c0b461f9448ef68067fe8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467052"
---
# <a name="submittime"></a><span data-ttu-id="850ff-103">SubmitTime</span><span class="sxs-lookup"><span data-stu-id="850ff-103">SubmitTime</span></span>

<span data-ttu-id="850ff-104">L’élément **SubmitTime** représente l’heure à laquelle le message a été envoyé au serveur.</span><span class="sxs-lookup"><span data-stu-id="850ff-104">The **SubmitTime** element represents the time at which the message was sent to the server.</span></span> 
  
```XML
<SubmitTime/>
```

 <span data-ttu-id="850ff-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="850ff-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="850ff-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="850ff-106">Attributes and elements</span></span>

<span data-ttu-id="850ff-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="850ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="850ff-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="850ff-108">Attributes</span></span>

<span data-ttu-id="850ff-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="850ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="850ff-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="850ff-110">Child elements</span></span>

<span data-ttu-id="850ff-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="850ff-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="850ff-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="850ff-112">Parent elements</span></span>

|<span data-ttu-id="850ff-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="850ff-113">**Element**</span></span>|<span data-ttu-id="850ff-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="850ff-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="850ff-115">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="850ff-115">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="850ff-116">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="850ff-116">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="850ff-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="850ff-117">Text value</span></span>

<span data-ttu-id="850ff-118">Une valeur de texte qui représente une date/heure est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="850ff-118">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="850ff-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="850ff-119">Remarks</span></span>

<span data-ttu-id="850ff-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="850ff-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="850ff-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="850ff-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="850ff-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="850ff-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="850ff-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="850ff-123">Schema Name</span></span>  <br/> |<span data-ttu-id="850ff-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="850ff-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="850ff-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="850ff-125">Validation File</span></span>  <br/> |<span data-ttu-id="850ff-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="850ff-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="850ff-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="850ff-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="850ff-128">False</span><span class="sxs-lookup"><span data-stu-id="850ff-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="850ff-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="850ff-129">See also</span></span>



[<span data-ttu-id="850ff-130">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="850ff-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="850ff-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="850ff-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

