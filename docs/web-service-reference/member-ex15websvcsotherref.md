---
title: Member
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
description: L’élément Member représente un membre d’une liste de distribution.
ms.openlocfilehash: e84223b7c41846ca2f174293bff46a8825777a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457304"
---
# <a name="member"></a><span data-ttu-id="9ef2d-103">Member</span><span class="sxs-lookup"><span data-stu-id="9ef2d-103">Member</span></span>

<span data-ttu-id="9ef2d-104">L’élément **member** représente un membre d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="9ef2d-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="9ef2d-105">**MemberType**</span><span class="sxs-lookup"><span data-stu-id="9ef2d-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9ef2d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9ef2d-106">Attributes and elements</span></span>

<span data-ttu-id="9ef2d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9ef2d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ef2d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9ef2d-108">Attributes</span></span>

|<span data-ttu-id="9ef2d-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9ef2d-109">**Attribute**</span></span>|<span data-ttu-id="9ef2d-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="9ef2d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9ef2d-111">Clé</span><span class="sxs-lookup"><span data-stu-id="9ef2d-111">Key</span></span>  <br/> |<span data-ttu-id="9ef2d-112">Fournit un identificateur unique pour le membre de la liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="9ef2d-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="9ef2d-113">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9ef2d-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9ef2d-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9ef2d-114">Child elements</span></span>

|<span data-ttu-id="9ef2d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9ef2d-115">**Element**</span></span>|<span data-ttu-id="9ef2d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="9ef2d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ef2d-117">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="9ef2d-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="9ef2d-118">Représente l’adresse de messagerie du membre de la liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="9ef2d-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="9ef2d-119">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9ef2d-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9ef2d-120">État (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="9ef2d-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="9ef2d-121">Fournit des informations sur l’état d’un membre de la liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="9ef2d-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="9ef2d-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9ef2d-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ef2d-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9ef2d-123">Parent elements</span></span>

|<span data-ttu-id="9ef2d-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9ef2d-124">**Element**</span></span>|<span data-ttu-id="9ef2d-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="9ef2d-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ef2d-126">Membres (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="9ef2d-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="9ef2d-127">Contient une liste de membres de liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="9ef2d-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9ef2d-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="9ef2d-128">Remarks</span></span>

<span data-ttu-id="9ef2d-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ef2d-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ef2d-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9ef2d-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ef2d-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9ef2d-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ef2d-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9ef2d-132">Schema Name</span></span>  <br/> |<span data-ttu-id="9ef2d-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9ef2d-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ef2d-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9ef2d-134">Validation File</span></span>  <br/> |<span data-ttu-id="9ef2d-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ef2d-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ef2d-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9ef2d-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ef2d-137">False</span><span class="sxs-lookup"><span data-stu-id="9ef2d-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ef2d-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9ef2d-138">See also</span></span>

- [<span data-ttu-id="9ef2d-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9ef2d-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

