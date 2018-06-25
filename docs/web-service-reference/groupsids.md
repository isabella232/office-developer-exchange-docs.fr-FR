---
title: GroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupSids
api_type:
- schema
ms.assetid: ebb00653-83f0-4080-a902-c38df6719800
description: L’élément GroupSids représente une collection d’identificateurs de sécurité Active Directory directory service groupe objet.
ms.openlocfilehash: c24c8ea3c3b7d37f41986997ed924c951b4a48ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827790"
---
# <a name="groupsids"></a><span data-ttu-id="731c3-103">GroupSids</span><span class="sxs-lookup"><span data-stu-id="731c3-103">GroupSids</span></span>

<span data-ttu-id="731c3-104">L’élément **GroupSids** représente une collection d’identificateurs de sécurité Active Directory directory service groupe objet.</span><span class="sxs-lookup"><span data-stu-id="731c3-104">The **GroupSids** element represents a collection of Active Directory directory service group object security identifiers.</span></span> 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 <span data-ttu-id="731c3-105">**NonEmptyArrayOfGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="731c3-105">**NonEmptyArrayOfGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="731c3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="731c3-106">Attributes and elements</span></span>

<span data-ttu-id="731c3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="731c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="731c3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="731c3-108">Attributes</span></span>

<span data-ttu-id="731c3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="731c3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="731c3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="731c3-110">Child elements</span></span>

|<span data-ttu-id="731c3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="731c3-111">**Element**</span></span>|<span data-ttu-id="731c3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="731c3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="731c3-113">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="731c3-113">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="731c3-114">Représente un identificateur de sécurité unique et un attribut pour un groupe d’objets Active Directory dont le compte est membre.</span><span class="sxs-lookup"><span data-stu-id="731c3-114">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="731c3-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="731c3-115">Parent elements</span></span>

|<span data-ttu-id="731c3-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="731c3-116">**Element**</span></span>|<span data-ttu-id="731c3-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="731c3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="731c3-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="731c3-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="731c3-119">Utilisé dans l’en-tête SOAP Simple Object Access Protocol () pour la sérialisation de jeton de l’authentification de serveur à serveur.</span><span class="sxs-lookup"><span data-stu-id="731c3-119">Used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="731c3-120">Sérialisation de jeton n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="731c3-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="731c3-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="731c3-121">Remarks</span></span>

<span data-ttu-id="731c3-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="731c3-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="731c3-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="731c3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="731c3-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="731c3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="731c3-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="731c3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="731c3-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="731c3-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="731c3-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="731c3-127">Validation File</span></span>  <br/> |<span data-ttu-id="731c3-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="731c3-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="731c3-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="731c3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="731c3-130">False</span><span class="sxs-lookup"><span data-stu-id="731c3-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="731c3-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="731c3-131">See also</span></span>



- [<span data-ttu-id="731c3-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="731c3-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

