---
title: IsSigned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsSigned
api_type:
- schema
ms.assetid: a4f90fe5-2834-4621-9aa3-b561f74d4674
description: L’élément IsSigned indique si les messages entrants doivent être connectés par ordre pour l’exception ou la condition à appliquer.
ms.openlocfilehash: 33ff204260465490c701c6573ff4140967ac625a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828105"
---
# <a name="issigned"></a><span data-ttu-id="59809-103">IsSigned</span><span class="sxs-lookup"><span data-stu-id="59809-103">IsSigned</span></span>

<span data-ttu-id="59809-104">L’élément **IsSigned** indique si les messages entrants doivent être connectés par ordre pour l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="59809-104">The **IsSigned** element indicates whether incoming messages must be signed in order for the condition or exception to apply.</span></span> 
  
```XML
<IsSigned>true | false</IsSigned>
```

 <span data-ttu-id="59809-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="59809-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59809-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59809-106">Attributes and elements</span></span>

<span data-ttu-id="59809-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59809-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59809-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="59809-108">Attributes</span></span>

<span data-ttu-id="59809-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59809-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59809-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59809-110">Child elements</span></span>

<span data-ttu-id="59809-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59809-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59809-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59809-112">Parent elements</span></span>

|<span data-ttu-id="59809-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59809-113">**Element**</span></span>|<span data-ttu-id="59809-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="59809-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59809-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="59809-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="59809-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="59809-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="59809-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="59809-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="59809-118">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="59809-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="59809-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="59809-119">Text value</span></span>

<span data-ttu-id="59809-120">Une valeur de texte de **la valeur true** indique que le message doit être connecté afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="59809-120">A text value of **true** indicates that the message must be signed in order for the condition or exception to apply.</span></span> <span data-ttu-id="59809-121">Texte la valeur **false** indique que le message n’a pas être connecté pour l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="59809-121">A text value of **false** indicates that the message does not have to be signed for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="59809-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="59809-122">Remarks</span></span>

<span data-ttu-id="59809-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="59809-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59809-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="59809-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59809-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="59809-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="59809-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="59809-126">Schema Name</span></span>  <br/> |<span data-ttu-id="59809-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="59809-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="59809-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="59809-128">Validation File</span></span>  <br/> |<span data-ttu-id="59809-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="59809-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="59809-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="59809-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="59809-131">True</span><span class="sxs-lookup"><span data-stu-id="59809-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59809-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59809-132">See also</span></span>



- [<span data-ttu-id="59809-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="59809-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

