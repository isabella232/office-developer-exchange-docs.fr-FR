---
title: ContainsSubjectOrBodyStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSubjectOrBodyStrings
api_type:
- schema
ms.assetid: 22aebf31-d9f4-4e03-bbff-c675409518d1
description: L’élément ContainsSubjectOrBodyStrings indique les chaînes qui doivent apparaître dans le corps ou l’objet des messages entrants pour que la condition ou l’exception s’applique.
ms.openlocfilehash: 6f9c7862912632e7e86a0b704e760c7fd0f5f14c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466821"
---
# <a name="containssubjectorbodystrings"></a><span data-ttu-id="cbe85-103">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="cbe85-103">ContainsSubjectOrBodyStrings</span></span>

<span data-ttu-id="cbe85-104">L’élément **ContainsSubjectOrBodyStrings** indique les chaînes qui doivent apparaître dans le corps ou l’objet des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="cbe85-104">The **ContainsSubjectOrBodyStrings** element indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectOrBodyStrings>
    <String/>
</ContainsSubjectOrBodyStrings>
```

 <span data-ttu-id="cbe85-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="cbe85-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cbe85-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cbe85-106">Attributes and elements</span></span>

<span data-ttu-id="cbe85-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cbe85-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cbe85-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cbe85-108">Attributes</span></span>

<span data-ttu-id="cbe85-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cbe85-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cbe85-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cbe85-110">Child elements</span></span>

|<span data-ttu-id="cbe85-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cbe85-111">**Element**</span></span>|<span data-ttu-id="cbe85-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="cbe85-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbe85-113">String</span><span class="sxs-lookup"><span data-stu-id="cbe85-113">String</span></span>](string.md) <br/> |<span data-ttu-id="cbe85-114">Représente une chaîne qui doit apparaître dans le corps ou l’objet des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="cbe85-114">Represents a string that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cbe85-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cbe85-115">Parent elements</span></span>

|<span data-ttu-id="cbe85-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cbe85-116">**Element**</span></span>|<span data-ttu-id="cbe85-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="cbe85-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbe85-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="cbe85-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="cbe85-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="cbe85-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="cbe85-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="cbe85-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="cbe85-121">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="cbe85-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cbe85-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cbe85-122">Text value</span></span>

<span data-ttu-id="cbe85-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cbe85-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cbe85-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="cbe85-124">Remarks</span></span>

<span data-ttu-id="cbe85-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cbe85-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cbe85-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cbe85-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cbe85-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cbe85-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cbe85-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cbe85-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cbe85-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="cbe85-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cbe85-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cbe85-130">Validation File</span></span>  <br/> |<span data-ttu-id="cbe85-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cbe85-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cbe85-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cbe85-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cbe85-133">True</span><span class="sxs-lookup"><span data-stu-id="cbe85-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cbe85-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cbe85-134">See also</span></span>



- [<span data-ttu-id="cbe85-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cbe85-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

