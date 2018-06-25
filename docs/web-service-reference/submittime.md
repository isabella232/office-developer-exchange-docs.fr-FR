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
ms.openlocfilehash: 3f19e2ac14b412ef8d1ab59eb069f0223cf782ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829617"
---
# <a name="submittime"></a><span data-ttu-id="3c90a-103">SubmitTime</span><span class="sxs-lookup"><span data-stu-id="3c90a-103">SubmitTime</span></span>

<span data-ttu-id="3c90a-104">L’élément **SubmitTime** représente l’heure à laquelle le message a été envoyé au serveur.</span><span class="sxs-lookup"><span data-stu-id="3c90a-104">The **SubmitTime** element represents the time at which the message was sent to the server.</span></span> 
  
```XML
<SubmitTime/>
```

 <span data-ttu-id="3c90a-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="3c90a-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c90a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3c90a-106">Attributes and elements</span></span>

<span data-ttu-id="3c90a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3c90a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c90a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3c90a-108">Attributes</span></span>

<span data-ttu-id="3c90a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3c90a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c90a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3c90a-110">Child elements</span></span>

<span data-ttu-id="3c90a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3c90a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3c90a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3c90a-112">Parent elements</span></span>

|<span data-ttu-id="3c90a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3c90a-113">**Element**</span></span>|<span data-ttu-id="3c90a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3c90a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c90a-115">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3c90a-115">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="3c90a-116">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="3c90a-116">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3c90a-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3c90a-117">Text value</span></span>

<span data-ttu-id="3c90a-118">Une valeur de texte qui représente une date/heure est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="3c90a-118">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3c90a-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="3c90a-119">Remarks</span></span>

<span data-ttu-id="3c90a-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c90a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c90a-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3c90a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c90a-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3c90a-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c90a-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3c90a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="3c90a-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3c90a-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c90a-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3c90a-125">Validation File</span></span>  <br/> |<span data-ttu-id="3c90a-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3c90a-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c90a-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3c90a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c90a-128">False</span><span class="sxs-lookup"><span data-stu-id="3c90a-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c90a-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3c90a-129">See also</span></span>



[<span data-ttu-id="3c90a-130">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3c90a-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="3c90a-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3c90a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

