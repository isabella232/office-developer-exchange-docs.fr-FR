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
ms.openlocfilehash: c95af4e09324e96f4551a05490dc200aec0cbd46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465365"
---
# <a name="restrictedgroupidentifier"></a><span data-ttu-id="9e5fb-103">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e5fb-103">RestrictedGroupIdentifier</span></span>

<span data-ttu-id="9e5fb-104">L’élément **RestrictGroupIdentifier** représente l’identificateur de sécurité (SID) de groupe et les attributs d’un groupe restreint au sein d’un jeton utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9e5fb-104">The **RestrictGroupIdentifier** element represents the group security identifier (SID) and attributes for a restricted group within a user token.</span></span> 
  
```xml
<RestrictedGroupIdentifier Attributes="">
   <SecurityIdentifier/>
</RestrictedGroupIdentifier>
```

 <span data-ttu-id="9e5fb-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="9e5fb-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e5fb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9e5fb-106">Attributes and elements</span></span>

<span data-ttu-id="9e5fb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9e5fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e5fb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9e5fb-108">Attributes</span></span>

|<span data-ttu-id="9e5fb-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9e5fb-109">**Attribute**</span></span>|<span data-ttu-id="9e5fb-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="9e5fb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9e5fb-111">**Attributs**</span><span class="sxs-lookup"><span data-stu-id="9e5fb-111">**Attributes**</span></span> <br/> |<span data-ttu-id="9e5fb-112">Contient les attributs de groupe.</span><span class="sxs-lookup"><span data-stu-id="9e5fb-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9e5fb-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9e5fb-113">Child elements</span></span>

|<span data-ttu-id="9e5fb-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9e5fb-114">**Element**</span></span>|<span data-ttu-id="9e5fb-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="9e5fb-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e5fb-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e5fb-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="9e5fb-117">Représente la forme SDDL (Security Descriptor Definition Language) d’un identificateur de sécurité.</span><span class="sxs-lookup"><span data-stu-id="9e5fb-117">Represents the security descriptor definition language (SDDL) form of a security identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e5fb-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9e5fb-118">Parent elements</span></span>

|<span data-ttu-id="9e5fb-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9e5fb-119">**Element**</span></span>|<span data-ttu-id="9e5fb-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="9e5fb-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e5fb-121">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="9e5fb-121">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="9e5fb-122">Représente une collection de groupes restreints au sein d’un jeton utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9e5fb-122">Represents a collection of restricted groups within a user token.</span></span> <span data-ttu-id="9e5fb-123">La sérialisation de jetons n’est pas prise en charge.</span><span class="sxs-lookup"><span data-stu-id="9e5fb-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9e5fb-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="9e5fb-124">Remarks</span></span>

<span data-ttu-id="9e5fb-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9e5fb-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e5fb-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9e5fb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e5fb-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9e5fb-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e5fb-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9e5fb-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9e5fb-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9e5fb-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="9e5fb-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9e5fb-130">Validation File</span></span>  <br/> |<span data-ttu-id="9e5fb-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9e5fb-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e5fb-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9e5fb-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e5fb-133">False</span><span class="sxs-lookup"><span data-stu-id="9e5fb-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e5fb-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9e5fb-134">See also</span></span>



- [<span data-ttu-id="9e5fb-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9e5fb-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

