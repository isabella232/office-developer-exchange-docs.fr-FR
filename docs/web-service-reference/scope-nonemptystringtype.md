---
title: Étendue (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Scope
api_type:
- schema
ms.assetid: 7efb6fd9-1615-469e-96f6-0f7846ad9b44
description: L’élément Scope spécifie l’étendue du rapport de suivi des messages.
ms.openlocfilehash: f86f6198e84e094e61ee569f6d005549316bbb9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466940"
---
# <a name="scope-nonemptystringtype"></a><span data-ttu-id="4510e-103">Étendue (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="4510e-103">Scope (NonEmptyStringType)</span></span>

<span data-ttu-id="4510e-104">L’élément **scope** spécifie l’étendue du rapport de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="4510e-104">The **Scope** element specifies the scope of the message tracking report.</span></span> 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 <span data-ttu-id="4510e-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="4510e-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4510e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4510e-106">Attributes and elements</span></span>

<span data-ttu-id="4510e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4510e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4510e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4510e-108">Attributes</span></span>

<span data-ttu-id="4510e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4510e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4510e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4510e-110">Child elements</span></span>

<span data-ttu-id="4510e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4510e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4510e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4510e-112">Parent elements</span></span>

<span data-ttu-id="4510e-113">[FindMessageTrackingReport](findmessagetrackingreport.md)  |  [GetMessageTrackingReport](getmessagetrackingreport.md)</span><span class="sxs-lookup"><span data-stu-id="4510e-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4510e-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4510e-114">Text value</span></span>

<span data-ttu-id="4510e-115">Le tableau suivant répertorie les valeurs possibles pour l’élément **scope** .</span><span class="sxs-lookup"><span data-stu-id="4510e-115">The following table lists the possible values for the **Scope** element.</span></span> 
  
|<span data-ttu-id="4510e-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4510e-116">**Value**</span></span>|<span data-ttu-id="4510e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="4510e-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4510e-118">Organisation</span><span class="sxs-lookup"><span data-stu-id="4510e-118">Organization</span></span>  <br/> |<span data-ttu-id="4510e-119">Les étendues de suivi des messages s’étendent au sein d’une organisation.</span><span class="sxs-lookup"><span data-stu-id="4510e-119">The message tracking scopes spans across an organization.</span></span>  <br/> |
|<span data-ttu-id="4510e-120">Forest (Forêt)</span><span class="sxs-lookup"><span data-stu-id="4510e-120">Forest</span></span>  <br/> |<span data-ttu-id="4510e-121">Les étendues de suivi des messages s’étendent dans une forêt.</span><span class="sxs-lookup"><span data-stu-id="4510e-121">The message tracking scopes spans across a forest.</span></span>  <br/> |
|<span data-ttu-id="4510e-122">Site</span><span class="sxs-lookup"><span data-stu-id="4510e-122">Site</span></span>  <br/> |<span data-ttu-id="4510e-123">Les étendues de suivi des messages s’étendent sur un site.</span><span class="sxs-lookup"><span data-stu-id="4510e-123">The message tracking scopes spans across a site.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4510e-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="4510e-124">Remarks</span></span>

<span data-ttu-id="4510e-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4510e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4510e-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4510e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4510e-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4510e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4510e-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4510e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="4510e-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4510e-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4510e-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4510e-130">Validation File</span></span>  <br/> |<span data-ttu-id="4510e-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4510e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4510e-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4510e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="4510e-133">False</span><span class="sxs-lookup"><span data-stu-id="4510e-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4510e-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4510e-134">See also</span></span>



- [<span data-ttu-id="4510e-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4510e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

