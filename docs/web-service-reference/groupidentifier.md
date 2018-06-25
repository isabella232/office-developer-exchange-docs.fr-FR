---
title: GroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIdentifier
api_type:
- schema
ms.assetid: bdc6fc1e-4979-42da-a35b-e3017988c7d3
description: L’élément GroupIdentifier représente un identificateur de sécurité unique et un attribut pour un groupe d’objets Active Directory directory service dont le compte est membre.
ms.openlocfilehash: d73d72979762238ca09496cfbd6636b4ff44a969
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827767"
---
# <a name="groupidentifier"></a><span data-ttu-id="85db4-103">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="85db4-103">GroupIdentifier</span></span>

<span data-ttu-id="85db4-104">L’élément **GroupIdentifier** représente un identificateur de sécurité unique et un attribut pour un groupe d’objets Active Directory directory service dont le compte est membre.</span><span class="sxs-lookup"><span data-stu-id="85db4-104">The **GroupIdentifier** element represents a single security identifier and attribute for an Active Directory directory service object group of which the account is a member.</span></span> 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 <span data-ttu-id="85db4-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="85db4-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85db4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="85db4-106">Attributes and elements</span></span>

<span data-ttu-id="85db4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="85db4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85db4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="85db4-108">Attributes</span></span>

|<span data-ttu-id="85db4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="85db4-109">**Attribute**</span></span>|<span data-ttu-id="85db4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="85db4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="85db4-111">**Attributes**</span><span class="sxs-lookup"><span data-stu-id="85db4-111">**Attributes**</span></span> <br/> |<span data-ttu-id="85db4-112">Contient les attributs d’un groupe.</span><span class="sxs-lookup"><span data-stu-id="85db4-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="85db4-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="85db4-113">Child elements</span></span>

|<span data-ttu-id="85db4-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85db4-114">**Element**</span></span>|<span data-ttu-id="85db4-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="85db4-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85db4-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="85db4-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="85db4-117">Représente le formulaire sécurité descripteur definition language (SDDL) d’un identificateur de sécurité ([SID](sid.md)) qui représente le groupe.</span><span class="sxs-lookup"><span data-stu-id="85db4-117">Represents the security descriptor definition language (SDDL) form of a security identifier ([SID](sid.md)) that represents the group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85db4-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="85db4-118">Parent elements</span></span>

|<span data-ttu-id="85db4-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85db4-119">**Element**</span></span>|<span data-ttu-id="85db4-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="85db4-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85db4-121">GroupSids</span><span class="sxs-lookup"><span data-stu-id="85db4-121">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="85db4-122">Représente une collection d’identificateurs de sécurité Active Directory groupe objet qui constituent un jeton de compte pour la sérialisation de jeton.</span><span class="sxs-lookup"><span data-stu-id="85db4-122">Represents a collection of Active Directory group object security identifiers that make up an account token for token serialization.</span></span> <span data-ttu-id="85db4-123">Sérialisation de jeton n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="85db4-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="85db4-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="85db4-124">Remarks</span></span>

<span data-ttu-id="85db4-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="85db4-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85db4-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="85db4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85db4-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="85db4-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85db4-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="85db4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="85db4-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="85db4-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="85db4-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="85db4-130">Validation File</span></span>  <br/> |<span data-ttu-id="85db4-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="85db4-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85db4-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="85db4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="85db4-133">False</span><span class="sxs-lookup"><span data-stu-id="85db4-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85db4-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="85db4-134">See also</span></span>



- [<span data-ttu-id="85db4-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="85db4-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

