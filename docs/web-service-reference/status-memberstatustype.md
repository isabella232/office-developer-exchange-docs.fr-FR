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
description: L’élément Status fournit des informations sur l’état d’un membre de liste de distribution sur le serveur.
ms.openlocfilehash: ef062433c80f0cca413c33012e1164b17e226faf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829580"
---
# <a name="status-memberstatustype"></a><span data-ttu-id="5486e-103">État (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="5486e-103">Status (MemberStatusType)</span></span>

<span data-ttu-id="5486e-104">L’élément **Status** fournit des informations sur l’état d’un membre de liste de distribution sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="5486e-104">The **Status** element provides information about the status of a distribution list member on the server.</span></span> 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 <span data-ttu-id="5486e-105">**MemberStatusType**</span><span class="sxs-lookup"><span data-stu-id="5486e-105">**MemberStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5486e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5486e-106">Attributes and elements</span></span>

<span data-ttu-id="5486e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5486e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5486e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5486e-108">Attributes</span></span>

<span data-ttu-id="5486e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5486e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5486e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5486e-110">Child elements</span></span>

<span data-ttu-id="5486e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5486e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5486e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5486e-112">Parent elements</span></span>

|<span data-ttu-id="5486e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5486e-113">**Element**</span></span>|<span data-ttu-id="5486e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5486e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5486e-115">Membre</span><span class="sxs-lookup"><span data-stu-id="5486e-115">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5486e-116">Représente un membre d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="5486e-116">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5486e-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5486e-117">Text value</span></span>

<span data-ttu-id="5486e-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **Status** .</span><span class="sxs-lookup"><span data-stu-id="5486e-118">The following table lists the possible values for the **Status** element.</span></span> 
  
<span data-ttu-id="5486e-119">**Valeurs des éléments de statut**</span><span class="sxs-lookup"><span data-stu-id="5486e-119">**Status element values**</span></span>

|<span data-ttu-id="5486e-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="5486e-120">**Value**</span></span>|<span data-ttu-id="5486e-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="5486e-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5486e-122">Non reconnu</span><span class="sxs-lookup"><span data-stu-id="5486e-122">Unrecognized</span></span>  <br/> |<span data-ttu-id="5486e-123">Informations sur les membres non valide ou non reconnu.</span><span class="sxs-lookup"><span data-stu-id="5486e-123">Member information is invalid or unrecognized.</span></span>  <br/> |
|<span data-ttu-id="5486e-124">Normal</span><span class="sxs-lookup"><span data-stu-id="5486e-124">Normal</span></span>  <br/> |<span data-ttu-id="5486e-125">Informations de membre dans une liste de distribution sont synchronisées avec l’objet référencé.</span><span class="sxs-lookup"><span data-stu-id="5486e-125">Member information in a distribution list is in sync with the referenced object.</span></span>  <br/> |
|<span data-ttu-id="5486e-126">Rétrogradé</span><span class="sxs-lookup"><span data-stu-id="5486e-126">Demoted</span></span>  <br/> |<span data-ttu-id="5486e-127">Objet référencé n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="5486e-127">Referenced object is not available.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5486e-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="5486e-128">Remarks</span></span>

<span data-ttu-id="5486e-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="5486e-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5486e-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5486e-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5486e-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5486e-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5486e-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5486e-132">Schema Name</span></span>  <br/> |<span data-ttu-id="5486e-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5486e-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="5486e-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5486e-134">Validation File</span></span>  <br/> |<span data-ttu-id="5486e-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5486e-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5486e-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5486e-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="5486e-137">False</span><span class="sxs-lookup"><span data-stu-id="5486e-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5486e-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5486e-138">See also</span></span>



- [<span data-ttu-id="5486e-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5486e-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

