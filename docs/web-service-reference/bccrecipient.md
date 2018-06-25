---
title: BccRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipient
api_type:
- schema
ms.assetid: 4ef0cff5-8a5a-4d76-9d2b-938774d8fc1b
description: L’élément BccRecipient représente un destinataire pour recevoir une copie carbone invisible (Cci) d’un message électronique.
ms.openlocfilehash: bed58536263196a61651493e92a4dcd1df3f5ec9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755376"
---
# <a name="bccrecipient"></a><span data-ttu-id="993d4-103">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="993d4-103">BccRecipient</span></span>

<span data-ttu-id="993d4-104">L’élément **BccRecipient** représente un destinataire pour recevoir une copie carbone invisible (Cci) d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="993d4-104">The **BccRecipient** element represents a recipient to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```XML
<BccRecipient>true | false</BccRecipient>
```

 <span data-ttu-id="993d4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="993d4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="993d4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="993d4-106">Attributes and elements</span></span>

<span data-ttu-id="993d4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="993d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="993d4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="993d4-108">Attributes</span></span>

<span data-ttu-id="993d4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="993d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="993d4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="993d4-110">Child elements</span></span>

<span data-ttu-id="993d4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="993d4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="993d4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="993d4-112">Parent elements</span></span>

|<span data-ttu-id="993d4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="993d4-113">**Element**</span></span>|<span data-ttu-id="993d4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="993d4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="993d4-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="993d4-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="993d4-116">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="993d4-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="993d4-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="993d4-117">Text value</span></span>

<span data-ttu-id="993d4-118">Cet élément peut être **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="993d4-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="993d4-119">La valeur **true** indique que le destinataire est carbone invisible copié ; la valeur **false** indique que le destinataire n’est pas copié de carbone invisible.</span><span class="sxs-lookup"><span data-stu-id="993d4-119">A value of **true** indicates that the recipient is blind carbon copied; a value of **false** indicates that the recipient is not blind carbon copied.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="993d4-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="993d4-120">Remarks</span></span>

<span data-ttu-id="993d4-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="993d4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="993d4-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="993d4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="993d4-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="993d4-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="993d4-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="993d4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="993d4-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="993d4-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="993d4-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="993d4-126">Validation File</span></span>  <br/> |<span data-ttu-id="993d4-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="993d4-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="993d4-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="993d4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="993d4-129">False</span><span class="sxs-lookup"><span data-stu-id="993d4-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="993d4-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="993d4-130">See also</span></span>



- [<span data-ttu-id="993d4-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="993d4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

