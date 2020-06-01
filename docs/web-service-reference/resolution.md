---
title: Résolution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Resolution
api_type:
- schema
ms.assetid: 573bed4b-d7b1-4baf-b16f-0795cdebf1a7
description: L’élément Resolution contient une seule entité résolue.
ms.openlocfilehash: 63c80f3c8d7dabf7e6dc1494df04c0be821b28bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468284"
---
# <a name="resolution"></a><span data-ttu-id="3f91f-103">Résolution</span><span class="sxs-lookup"><span data-stu-id="3f91f-103">Resolution</span></span>

<span data-ttu-id="3f91f-104">L’élément **Resolution** contient une seule entité résolue.</span><span class="sxs-lookup"><span data-stu-id="3f91f-104">The **Resolution** element contains a single resolved entity.</span></span> 
  
[<span data-ttu-id="3f91f-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="3f91f-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="3f91f-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3f91f-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="3f91f-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3f91f-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="3f91f-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="3f91f-108">ResolutionSet</span></span>](resolutionset.md)
  
[<span data-ttu-id="3f91f-109">Solution</span><span class="sxs-lookup"><span data-stu-id="3f91f-109">Resolution</span></span>](resolution.md)
  
```xml
<Resolution>
   <Mailbox/>
   <Contact/>
</Resolution>
```

 <span data-ttu-id="3f91f-110">**ResolutionType**</span><span class="sxs-lookup"><span data-stu-id="3f91f-110">**ResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f91f-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3f91f-111">Attributes and elements</span></span>

<span data-ttu-id="3f91f-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3f91f-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f91f-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="3f91f-113">Attributes</span></span>

<span data-ttu-id="3f91f-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3f91f-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f91f-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3f91f-115">Child elements</span></span>

|<span data-ttu-id="3f91f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3f91f-116">**Element**</span></span>|<span data-ttu-id="3f91f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="3f91f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f91f-118">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="3f91f-118">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="3f91f-119">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3f91f-119">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
|[<span data-ttu-id="3f91f-120">Contact</span><span class="sxs-lookup"><span data-stu-id="3f91f-120">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="3f91f-121">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f91f-121">Represents an Exchange contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f91f-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3f91f-122">Parent elements</span></span>

|<span data-ttu-id="3f91f-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3f91f-123">**Element**</span></span>|<span data-ttu-id="3f91f-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="3f91f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f91f-125">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="3f91f-125">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="3f91f-126">Contient un tableau de résolutions pour un nom ambigu.</span><span class="sxs-lookup"><span data-stu-id="3f91f-126">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3f91f-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="3f91f-127">Remarks</span></span>

<span data-ttu-id="3f91f-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3f91f-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f91f-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3f91f-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f91f-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3f91f-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f91f-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3f91f-131">Schema name</span></span>  <br/> |<span data-ttu-id="3f91f-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3f91f-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="3f91f-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3f91f-133">Validation file</span></span>  <br/> |<span data-ttu-id="3f91f-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3f91f-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f91f-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3f91f-135">Can be empty</span></span>  <br/> |<span data-ttu-id="3f91f-136">False</span><span class="sxs-lookup"><span data-stu-id="3f91f-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f91f-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3f91f-137">See also</span></span>



[<span data-ttu-id="3f91f-138">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="3f91f-138">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="3f91f-139">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="3f91f-139">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="3f91f-140">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="3f91f-140">ResolveNames operation</span></span>](resolvenames-operation.md)

