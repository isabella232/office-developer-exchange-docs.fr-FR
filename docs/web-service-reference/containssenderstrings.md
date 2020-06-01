---
title: ContainsSenderStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSenderStrings
api_type:
- schema
ms.assetid: 3e16163f-cffe-4c4e-9a2a-00245d25ba96
description: L’élément ContainsSenderStrings indique les chaînes qui doivent apparaître dans la propriété from des messages entrants pour que la condition ou l’exception s’applique.
ms.openlocfilehash: e7b78f1311d288db7969a0024bde84433e18d37f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458977"
---
# <a name="containssenderstrings"></a><span data-ttu-id="b9118-103">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="b9118-103">ContainsSenderStrings</span></span>

<span data-ttu-id="b9118-104">L’élément **ContainsSenderStrings** indique les chaînes qui doivent apparaître dans la propriété **from** des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="b9118-104">The **ContainsSenderStrings** element indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSenderStrings>
    <String/>
</ContainsSenderStrings>
```

 <span data-ttu-id="b9118-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="b9118-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9118-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b9118-106">Attributes and elements</span></span>

<span data-ttu-id="b9118-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b9118-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9118-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b9118-108">Attributes</span></span>

<span data-ttu-id="b9118-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b9118-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9118-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b9118-110">Child elements</span></span>

|<span data-ttu-id="b9118-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b9118-111">**Element**</span></span>|<span data-ttu-id="b9118-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b9118-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9118-113">String</span><span class="sxs-lookup"><span data-stu-id="b9118-113">String</span></span>](string.md) <br/> |<span data-ttu-id="b9118-114">Représente une chaîne qui doit apparaître dans la propriété **from** des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="b9118-114">Represents a string that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b9118-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b9118-115">Parent elements</span></span>

|<span data-ttu-id="b9118-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b9118-116">**Element**</span></span>|<span data-ttu-id="b9118-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b9118-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9118-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="b9118-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="b9118-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="b9118-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="b9118-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="b9118-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="b9118-121">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="b9118-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9118-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b9118-122">Text value</span></span>

<span data-ttu-id="b9118-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b9118-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b9118-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="b9118-124">Remarks</span></span>

<span data-ttu-id="b9118-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9118-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9118-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b9118-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9118-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b9118-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b9118-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b9118-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b9118-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b9118-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b9118-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b9118-130">Validation File</span></span>  <br/> |<span data-ttu-id="b9118-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b9118-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b9118-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b9118-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9118-133">True</span><span class="sxs-lookup"><span data-stu-id="b9118-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9118-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b9118-134">See also</span></span>



- [<span data-ttu-id="b9118-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b9118-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

