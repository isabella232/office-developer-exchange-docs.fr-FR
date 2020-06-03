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
description: L’élément GroupIdentifier représente un identificateur de sécurité et un attribut uniques pour un groupe d’objets de service d’annuaire Active Directory dont le compte est membre.
ms.openlocfilehash: 8b427b9228cc5e66f46f70389acf2fa4bcd283b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530802"
---
# <a name="groupidentifier"></a><span data-ttu-id="0c1eb-103">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c1eb-103">GroupIdentifier</span></span>

<span data-ttu-id="0c1eb-104">L’élément **GroupIdentifier** représente un identificateur de sécurité et un attribut uniques pour un groupe d’objets de service d’annuaire Active Directory dont le compte est membre.</span><span class="sxs-lookup"><span data-stu-id="0c1eb-104">The **GroupIdentifier** element represents a single security identifier and attribute for an Active Directory directory service object group of which the account is a member.</span></span> 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 <span data-ttu-id="0c1eb-105">**SidAndAttributesType**</span><span class="sxs-lookup"><span data-stu-id="0c1eb-105">**SidAndAttributesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c1eb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0c1eb-106">Attributes and elements</span></span>

<span data-ttu-id="0c1eb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0c1eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c1eb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0c1eb-108">Attributes</span></span>

|<span data-ttu-id="0c1eb-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="0c1eb-109">**Attribute**</span></span>|<span data-ttu-id="0c1eb-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="0c1eb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0c1eb-111">**Attributs**</span><span class="sxs-lookup"><span data-stu-id="0c1eb-111">**Attributes**</span></span> <br/> |<span data-ttu-id="0c1eb-112">Contient les attributs de groupe.</span><span class="sxs-lookup"><span data-stu-id="0c1eb-112">Contains group attributes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0c1eb-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0c1eb-113">Child elements</span></span>

|<span data-ttu-id="0c1eb-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0c1eb-114">**Element**</span></span>|<span data-ttu-id="0c1eb-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="0c1eb-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c1eb-116">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c1eb-116">SecurityIdentifier</span></span>](securityidentifier.md) <br/> |<span data-ttu-id="0c1eb-117">Représente la forme SDDL (Security Descriptor Definition Language) d’un identificateur de sécurité ([sid](sid.md)) qui représente le groupe.</span><span class="sxs-lookup"><span data-stu-id="0c1eb-117">Represents the security descriptor definition language (SDDL) form of a security identifier ([SID](sid.md)) that represents the group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c1eb-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0c1eb-118">Parent elements</span></span>

|<span data-ttu-id="0c1eb-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0c1eb-119">**Element**</span></span>|<span data-ttu-id="0c1eb-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="0c1eb-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c1eb-121">GroupSids</span><span class="sxs-lookup"><span data-stu-id="0c1eb-121">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="0c1eb-122">Représente une collection d’identificateurs de sécurité d’objets de groupe Active Directory qui constituent un jeton de compte pour la sérialisation de jetons.</span><span class="sxs-lookup"><span data-stu-id="0c1eb-122">Represents a collection of Active Directory group object security identifiers that make up an account token for token serialization.</span></span> <span data-ttu-id="0c1eb-123">La sérialisation de jetons n’est pas prise en charge.</span><span class="sxs-lookup"><span data-stu-id="0c1eb-123">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0c1eb-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="0c1eb-124">Remarks</span></span>

<span data-ttu-id="0c1eb-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0c1eb-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c1eb-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0c1eb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c1eb-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0c1eb-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0c1eb-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0c1eb-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0c1eb-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0c1eb-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="0c1eb-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0c1eb-130">Validation File</span></span>  <br/> |<span data-ttu-id="0c1eb-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0c1eb-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0c1eb-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0c1eb-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c1eb-133">False</span><span class="sxs-lookup"><span data-stu-id="0c1eb-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c1eb-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0c1eb-134">See also</span></span>



- [<span data-ttu-id="0c1eb-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0c1eb-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

