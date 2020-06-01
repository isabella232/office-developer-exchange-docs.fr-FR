---
title: MessageClassifications
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageClassifications
api_type:
- schema
ms.assetid: 041b3d48-8f43-47f3-869f-72b66bef372a
description: L’élément MessageClassifications représente les classifications de message qui doivent être marquées sur les messages entrants pour que la condition ou l’exception s’applique.
ms.openlocfilehash: 63481aa8903c4e9637870130eb9154118471c3b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467969"
---
# <a name="messageclassifications"></a><span data-ttu-id="34924-103">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="34924-103">MessageClassifications</span></span>

<span data-ttu-id="34924-104">L’élément **MessageClassifications** représente les classifications de message qui doivent être marquées sur les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="34924-104">The **MessageClassifications** element represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<MessageClassifications>
    <String/>
</MessageClassifications>
```

 <span data-ttu-id="34924-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="34924-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34924-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="34924-106">Attributes and elements</span></span>

<span data-ttu-id="34924-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="34924-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34924-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="34924-108">Attributes</span></span>

<span data-ttu-id="34924-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="34924-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34924-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="34924-110">Child elements</span></span>

|<span data-ttu-id="34924-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="34924-111">**Element**</span></span>|<span data-ttu-id="34924-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="34924-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34924-113">String</span><span class="sxs-lookup"><span data-stu-id="34924-113">String</span></span>](string.md) <br/> |<span data-ttu-id="34924-114">Représente une classification de message.</span><span class="sxs-lookup"><span data-stu-id="34924-114">Represents a message classification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="34924-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="34924-115">Parent elements</span></span>

|<span data-ttu-id="34924-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="34924-116">**Element**</span></span>|<span data-ttu-id="34924-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="34924-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34924-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="34924-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="34924-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="34924-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="34924-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="34924-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="34924-121">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="34924-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="34924-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="34924-122">Text value</span></span>

<span data-ttu-id="34924-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="34924-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="34924-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="34924-124">Remarks</span></span>

<span data-ttu-id="34924-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="34924-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34924-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="34924-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34924-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="34924-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="34924-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="34924-128">Schema Name</span></span>  <br/> |<span data-ttu-id="34924-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="34924-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="34924-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="34924-130">Validation File</span></span>  <br/> |<span data-ttu-id="34924-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="34924-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="34924-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="34924-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="34924-133">True</span><span class="sxs-lookup"><span data-stu-id="34924-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34924-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="34924-134">See also</span></span>



- [<span data-ttu-id="34924-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="34924-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

