---
title: RestrictedGroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RestrictedGroupIdentifier
api_type:
- schema
ms.assetid: a3ea3c81-9f99-4836-8cb4-2384ea63f093
description: L’élément RestrictGroupIdentifier représente l’identificateur de sécurité (SID) de groupe et les attributs d’un groupe restreint au sein d’un jeton utilisateur.
ms.openlocfilehash: c6db8672b2afa855e83f2e9a2bf84c9ff33bdc7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829206"
---
# <a name="restrictedgroupidentifier"></a><span data-ttu-id="5965f-103">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="5965f-103">RestrictedGroupIdentifier</span></span>

<span data-ttu-id="5965f-104">L’élément **RestrictGroupIdentifier** représente l’identificateur de sécurité (SID) de groupe et les attributs d’un groupe restreint au sein d’un jeton utilisateur.</span><span class="sxs-lookup"><span data-stu-id="5965f-104">The **RestrictGroupIdentifier** element represents the group security identifier (SID) and attributes for a restricted group within a user token.</span></span> 
  
```xml
<RestrictedGroupIdentifier Attributes="">
   <SecurityIdentifier/>
</RestrictedGroupIdentifier>
```

 <span data-ttu-id="5965f-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="5965f-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5965f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5965f-106">Attributes and elements</span></span>

<span data-ttu-id="5965f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5965f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5965f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5965f-108">Attributes</span></span>

|<span data-ttu-id="5965f-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="5965f-109">**Attribute**</span></span>|<span data-ttu-id="5965f-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="5965f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5965f-111">**Attributes**</span><span class="sxs-lookup"><span data-stu-id="5965f-111">**Attributes**</span></span> <br/> |<span data-ttu-id="5965f-112">Contient les attributs d’un groupe.</span><span class="sxs-lookup"><span data-stu-id="5965f-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5965f-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5965f-113">Child elements</span></span>

|<span data-ttu-id="5965f-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5965f-114">**Element**</span></span>|<span data-ttu-id="5965f-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="5965f-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5965f-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="5965f-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="5965f-117">Représente le formulaire sécurité descripteur definition language (SDDL) d’un identificateur de sécurité.</span><span class="sxs-lookup"><span data-stu-id="5965f-117">Represents the security descriptor definition language (SDDL) form of a security identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5965f-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5965f-118">Parent elements</span></span>

|<span data-ttu-id="5965f-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5965f-119">**Element**</span></span>|<span data-ttu-id="5965f-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="5965f-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5965f-121">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="5965f-121">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="5965f-122">Représente une collection de groupes restreints au sein d’un jeton utilisateur.</span><span class="sxs-lookup"><span data-stu-id="5965f-122">Represents a collection of restricted groups within a user token.</span></span> <span data-ttu-id="5965f-123">Sérialisation de jeton n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="5965f-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5965f-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="5965f-124">Remarks</span></span>

<span data-ttu-id="5965f-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5965f-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5965f-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5965f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5965f-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5965f-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5965f-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5965f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5965f-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5965f-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="5965f-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5965f-130">Validation File</span></span>  <br/> |<span data-ttu-id="5965f-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5965f-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5965f-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5965f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5965f-133">False</span><span class="sxs-lookup"><span data-stu-id="5965f-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5965f-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5965f-134">See also</span></span>



- [<span data-ttu-id="5965f-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5965f-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

