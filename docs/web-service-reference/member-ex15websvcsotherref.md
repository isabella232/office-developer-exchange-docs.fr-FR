---
title: Membre
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Member
api_type:
- schema
ms.assetid: af9c5ff8-02a4-41fc-876d-14ac05f1ee77
description: L’élément membre représente un membre d’une liste de distribution.
ms.openlocfilehash: c38e2ed24e78b5199d4d65cce27a00a8e6704037
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19828434"
---
# <a name="member"></a><span data-ttu-id="d8b37-103">Membre</span><span class="sxs-lookup"><span data-stu-id="d8b37-103">Member</span></span>

<span data-ttu-id="d8b37-104">L’élément **membre** représente un membre d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="d8b37-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="d8b37-105">**MemberType**</span><span class="sxs-lookup"><span data-stu-id="d8b37-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d8b37-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d8b37-106">Attributes and elements</span></span>

<span data-ttu-id="d8b37-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d8b37-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8b37-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d8b37-108">Attributes</span></span>

|<span data-ttu-id="d8b37-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d8b37-109">**Attribute**</span></span>|<span data-ttu-id="d8b37-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8b37-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d8b37-111">Clé</span><span class="sxs-lookup"><span data-stu-id="d8b37-111">Key</span></span>  <br/> |<span data-ttu-id="d8b37-112">Fournit un identificateur unique pour le membre de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="d8b37-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="d8b37-113">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d8b37-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d8b37-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d8b37-114">Child elements</span></span>

|<span data-ttu-id="d8b37-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d8b37-115">**Element**</span></span>|<span data-ttu-id="d8b37-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8b37-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8b37-117">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="d8b37-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="d8b37-118">Représente l’adresse de messagerie du membre de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="d8b37-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="d8b37-119">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d8b37-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d8b37-120">État (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="d8b37-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="d8b37-121">Fournit des informations sur l’état d’un membre de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="d8b37-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="d8b37-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d8b37-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8b37-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d8b37-123">Parent elements</span></span>

|<span data-ttu-id="d8b37-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d8b37-124">**Element**</span></span>|<span data-ttu-id="d8b37-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8b37-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8b37-126">Membres (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="d8b37-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="d8b37-127">Contient une liste de membres de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="d8b37-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d8b37-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="d8b37-128">Remarks</span></span>

<span data-ttu-id="d8b37-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8b37-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8b37-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d8b37-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8b37-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d8b37-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8b37-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d8b37-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d8b37-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d8b37-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8b37-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d8b37-134">Validation File</span></span>  <br/> |<span data-ttu-id="d8b37-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d8b37-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8b37-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d8b37-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8b37-137">False</span><span class="sxs-lookup"><span data-stu-id="d8b37-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8b37-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d8b37-138">See also</span></span>

- [<span data-ttu-id="d8b37-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d8b37-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

