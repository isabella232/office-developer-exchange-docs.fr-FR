---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: L’élément DisableReason spécifie la raison pour laquelle vous désactivez une application.
ms.openlocfilehash: 1406d69647bde5389dc9bb61adf7537a57d5adfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463670"
---
# <a name="disablereason"></a><span data-ttu-id="55776-103">DisableReason</span><span class="sxs-lookup"><span data-stu-id="55776-103">DisableReason</span></span>

<span data-ttu-id="55776-104">L’élément **DisableReason** spécifie la raison pour laquelle vous désactivez une application.</span><span class="sxs-lookup"><span data-stu-id="55776-104">The **DisableReason** element specifies the reason for disabling an app.</span></span> 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 <span data-ttu-id="55776-105">**DisableReasonType**</span><span class="sxs-lookup"><span data-stu-id="55776-105">**DisableReasonType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55776-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="55776-106">Attributes and elements</span></span>

<span data-ttu-id="55776-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="55776-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55776-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="55776-108">Attributes</span></span>

<span data-ttu-id="55776-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="55776-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55776-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="55776-110">Child elements</span></span>

<span data-ttu-id="55776-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="55776-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55776-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="55776-112">Parent elements</span></span>

|<span data-ttu-id="55776-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="55776-113">**Element**</span></span>|<span data-ttu-id="55776-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="55776-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55776-115">DisableApp</span><span class="sxs-lookup"><span data-stu-id="55776-115">DisableApp</span></span>](disableapp.md) <br/> |<span data-ttu-id="55776-116">Spécifie une demande de désactivation d’une application.</span><span class="sxs-lookup"><span data-stu-id="55776-116">Specifies a request to disable an app.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55776-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="55776-117">Text value</span></span>

<span data-ttu-id="55776-118">**Valeur de texte de l’élément DisableReason**</span><span class="sxs-lookup"><span data-stu-id="55776-118">**DisableReason element text value**</span></span>

|<span data-ttu-id="55776-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="55776-119">**Value**</span></span>|<span data-ttu-id="55776-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="55776-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="55776-121">Noreason</span><span class="sxs-lookup"><span data-stu-id="55776-121">NoReason</span></span>  <br/> |<span data-ttu-id="55776-122">Aucune raison donnée</span><span class="sxs-lookup"><span data-stu-id="55776-122">No reason given</span></span>  <br/> |
|<span data-ttu-id="55776-123">OutlookClientPerformance</span><span class="sxs-lookup"><span data-stu-id="55776-123">OutlookClientPerformance</span></span>  <br/> |<span data-ttu-id="55776-124">Pour améliorer les performances des clients de messagerie.</span><span class="sxs-lookup"><span data-stu-id="55776-124">To improve email client performance.</span></span>  <br/> |
|<span data-ttu-id="55776-125">OWAClientPerformance</span><span class="sxs-lookup"><span data-stu-id="55776-125">OWAClientPerformance</span></span>  <br/> |<span data-ttu-id="55776-126">Pour améliorer les performances du client Web App.</span><span class="sxs-lookup"><span data-stu-id="55776-126">To improve Web app client performance.</span></span>  <br/> |
|<span data-ttu-id="55776-127">MobileClientPerformance</span><span class="sxs-lookup"><span data-stu-id="55776-127">MobileClientPerformance</span></span>  <br/> |<span data-ttu-id="55776-128">Pour améliorer les performances des clients mobiles.</span><span class="sxs-lookup"><span data-stu-id="55776-128">To improve mobile client performance.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55776-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="55776-129">Remarks</span></span>

<span data-ttu-id="55776-130">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="55776-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="55776-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="55776-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55776-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="55776-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55776-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="55776-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55776-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="55776-134">Schema Name</span></span>  <br/> |<span data-ttu-id="55776-135">Schéma type</span><span class="sxs-lookup"><span data-stu-id="55776-135">Type schema</span></span>  <br/> |
|<span data-ttu-id="55776-136">Validation File</span><span class="sxs-lookup"><span data-stu-id="55776-136">Validation File</span></span>  <br/> |<span data-ttu-id="55776-137">types. xsd</span><span class="sxs-lookup"><span data-stu-id="55776-137">types.xsd</span></span>  <br/> |
|<span data-ttu-id="55776-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="55776-138">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="55776-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="55776-139">See also</span></span>

- [<span data-ttu-id="55776-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="55776-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

