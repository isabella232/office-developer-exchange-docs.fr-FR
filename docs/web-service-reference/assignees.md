---
title: Intervenants
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20ef18c2-daa0-4f65-a515-e84e9993a77f
description: L’élément intervenants spécifie les personnes auxquels une tâche est affectée.
ms.openlocfilehash: 5fc301cd77268213e95fd33a2a2f36dbe218b512
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755327"
---
# <a name="assignees"></a><span data-ttu-id="46336-103">Intervenants</span><span class="sxs-lookup"><span data-stu-id="46336-103">Assignees</span></span>

<span data-ttu-id="46336-104">L’élément **intervenants** spécifie les personnes auxquels une tâche est affectée.</span><span class="sxs-lookup"><span data-stu-id="46336-104">The **Assignees** element specifies the people to whom a task is assigned.</span></span> 
  
```XML
<Assignees>
    <Name></Name>
    <UserID></UserID>
</Assignees>
```

 <span data-ttu-id="46336-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="46336-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46336-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="46336-106">Attributes and elements</span></span>

<span data-ttu-id="46336-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="46336-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46336-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="46336-108">Attributes</span></span>

<span data-ttu-id="46336-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="46336-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46336-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="46336-110">Child elements</span></span>

|<span data-ttu-id="46336-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="46336-111">**Element**</span></span>|<span data-ttu-id="46336-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="46336-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46336-113">Nom (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="46336-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="46336-114">Représente le nom complet de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="46336-114">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="46336-115">Nom d’utilisateur (chaîne)</span><span class="sxs-lookup"><span data-stu-id="46336-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="46336-116">Spécifie l’identificateur d’utilisateur d’un utilisateur de messagerie.</span><span class="sxs-lookup"><span data-stu-id="46336-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46336-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="46336-117">Parent elements</span></span>

|<span data-ttu-id="46336-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="46336-118">**Element**</span></span>|<span data-ttu-id="46336-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="46336-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46336-120">TaskSuggestion</span><span class="sxs-lookup"><span data-stu-id="46336-120">TaskSuggestion</span></span>](tasksuggestion.md) <br/> |<span data-ttu-id="46336-121">Spécifie une tâche proposée.</span><span class="sxs-lookup"><span data-stu-id="46336-121">Specifies a proposed task.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46336-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="46336-122">Remarks</span></span>

<span data-ttu-id="46336-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="46336-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="46336-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="46336-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46336-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="46336-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46336-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="46336-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46336-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="46336-127">Schema Name</span></span>  <br/> |<span data-ttu-id="46336-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="46336-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="46336-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="46336-129">Validation File</span></span>  <br/> |<span data-ttu-id="46336-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="46336-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="46336-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="46336-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="46336-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="46336-132">See also</span></span>

- [<span data-ttu-id="46336-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="46336-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

