---
title: ContainsHeaderStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsHeaderStrings
api_type:
- schema
ms.assetid: 5f68427b-990a-4a27-bfb3-fce3115b02d7
description: L’élément ContainsHeaderStrings indique les chaînes qui doivent apparaître dans les en-têtes des messages entrants pour que la condition ou l’exception s’applique.
ms.openlocfilehash: 23e3d0e7cff9c78edbac10a6275514af93cab325
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458991"
---
# <a name="containsheaderstrings"></a><span data-ttu-id="e3fbe-103">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="e3fbe-103">ContainsHeaderStrings</span></span>

<span data-ttu-id="e3fbe-104">L’élément **ContainsHeaderStrings** indique les chaînes qui doivent apparaître dans les en-têtes des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="e3fbe-104">The **ContainsHeaderStrings** element indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsHeaderStrings>
    <String/>
</ContainsHeaderStrings>
```

 <span data-ttu-id="e3fbe-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="e3fbe-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3fbe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e3fbe-106">Attributes and elements</span></span>

<span data-ttu-id="e3fbe-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e3fbe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3fbe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e3fbe-108">Attributes</span></span>

<span data-ttu-id="e3fbe-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e3fbe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3fbe-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e3fbe-110">Child elements</span></span>

|<span data-ttu-id="e3fbe-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e3fbe-111">**Element**</span></span>|<span data-ttu-id="e3fbe-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e3fbe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3fbe-113">String</span><span class="sxs-lookup"><span data-stu-id="e3fbe-113">String</span></span>](string.md) <br/> |<span data-ttu-id="e3fbe-114">Représente une chaîne qui doit apparaître dans les en-têtes des messages pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="e3fbe-114">Represents a string that must appear in message headers in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3fbe-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e3fbe-115">Parent elements</span></span>

|<span data-ttu-id="e3fbe-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e3fbe-116">**Element**</span></span>|<span data-ttu-id="e3fbe-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="e3fbe-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3fbe-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="e3fbe-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="e3fbe-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="e3fbe-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="e3fbe-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="e3fbe-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="e3fbe-121">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="e3fbe-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e3fbe-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e3fbe-122">Text value</span></span>

<span data-ttu-id="e3fbe-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e3fbe-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e3fbe-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="e3fbe-124">Remarks</span></span>

<span data-ttu-id="e3fbe-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e3fbe-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3fbe-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e3fbe-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3fbe-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e3fbe-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e3fbe-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e3fbe-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e3fbe-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e3fbe-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e3fbe-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e3fbe-130">Validation File</span></span>  <br/> |<span data-ttu-id="e3fbe-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e3fbe-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e3fbe-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e3fbe-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3fbe-133">True</span><span class="sxs-lookup"><span data-stu-id="e3fbe-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3fbe-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e3fbe-134">See also</span></span>



- [<span data-ttu-id="e3fbe-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e3fbe-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

