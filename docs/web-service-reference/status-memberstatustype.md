---
title: État (MemberStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 4f8a860b-0a48-4a0d-9a7a-69a0304aa747
description: L’élément Status fournit des informations sur l’état d’un membre de la liste de distribution sur le serveur.
ms.openlocfilehash: bfa0c349d6af51c1b2238c9749d2656541d31906
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465463"
---
# <a name="status-memberstatustype"></a><span data-ttu-id="2b5e7-103">État (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="2b5e7-103">Status (MemberStatusType)</span></span>

<span data-ttu-id="2b5e7-104">L’élément **Status** fournit des informations sur l’état d’un membre de la liste de distribution sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="2b5e7-104">The **Status** element provides information about the status of a distribution list member on the server.</span></span> 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 <span data-ttu-id="2b5e7-105">**MemberStatusType**</span><span class="sxs-lookup"><span data-stu-id="2b5e7-105">**MemberStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b5e7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2b5e7-106">Attributes and elements</span></span>

<span data-ttu-id="2b5e7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2b5e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b5e7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2b5e7-108">Attributes</span></span>

<span data-ttu-id="2b5e7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2b5e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b5e7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2b5e7-110">Child elements</span></span>

<span data-ttu-id="2b5e7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2b5e7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b5e7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2b5e7-112">Parent elements</span></span>

|<span data-ttu-id="2b5e7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2b5e7-113">**Element**</span></span>|<span data-ttu-id="2b5e7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b5e7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b5e7-115">Membre</span><span class="sxs-lookup"><span data-stu-id="2b5e7-115">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2b5e7-116">Représente un membre d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="2b5e7-116">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2b5e7-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2b5e7-117">Text value</span></span>

<span data-ttu-id="2b5e7-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **Status** .</span><span class="sxs-lookup"><span data-stu-id="2b5e7-118">The following table lists the possible values for the **Status** element.</span></span> 
  
<span data-ttu-id="2b5e7-119">**Valeurs de l’élément Status**</span><span class="sxs-lookup"><span data-stu-id="2b5e7-119">**Status element values**</span></span>

|<span data-ttu-id="2b5e7-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="2b5e7-120">**Value**</span></span>|<span data-ttu-id="2b5e7-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b5e7-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2b5e7-122">Non reconnu</span><span class="sxs-lookup"><span data-stu-id="2b5e7-122">Unrecognized</span></span>  <br/> |<span data-ttu-id="2b5e7-123">Les informations de membre ne sont pas valides ou ne sont pas reconnues.</span><span class="sxs-lookup"><span data-stu-id="2b5e7-123">Member information is invalid or unrecognized.</span></span>  <br/> |
|<span data-ttu-id="2b5e7-124">Normal</span><span class="sxs-lookup"><span data-stu-id="2b5e7-124">Normal</span></span>  <br/> |<span data-ttu-id="2b5e7-125">Les informations sur les membres d’une liste de distribution sont synchronisées avec l’objet référencé.</span><span class="sxs-lookup"><span data-stu-id="2b5e7-125">Member information in a distribution list is in sync with the referenced object.</span></span>  <br/> |
|<span data-ttu-id="2b5e7-126">Rétrogradé</span><span class="sxs-lookup"><span data-stu-id="2b5e7-126">Demoted</span></span>  <br/> |<span data-ttu-id="2b5e7-127">L’objet référencé n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="2b5e7-127">Referenced object is not available.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2b5e7-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="2b5e7-128">Remarks</span></span>

<span data-ttu-id="2b5e7-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2b5e7-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b5e7-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2b5e7-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b5e7-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2b5e7-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b5e7-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2b5e7-132">Schema Name</span></span>  <br/> |<span data-ttu-id="2b5e7-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2b5e7-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b5e7-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2b5e7-134">Validation File</span></span>  <br/> |<span data-ttu-id="2b5e7-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b5e7-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b5e7-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2b5e7-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="2b5e7-137">False</span><span class="sxs-lookup"><span data-stu-id="2b5e7-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b5e7-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2b5e7-138">See also</span></span>



- [<span data-ttu-id="2b5e7-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2b5e7-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

