---
title: RestrictedGroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RestrictedGroupSids
api_type:
- schema
ms.assetid: 569ab552-5616-444a-a7f5-de366a684a34
description: L’élément RestrictedGroupSids représente une collection de groupes restreints à partir d’un jeton d’utilisateur.
ms.openlocfilehash: fcfee809261c7ed0a4e0d092c091841fec641e46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829201"
---
# <a name="restrictedgroupsids"></a><span data-ttu-id="20547-103">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="20547-103">RestrictedGroupSids</span></span>

<span data-ttu-id="20547-104">L’élément **RestrictedGroupSids** représente une collection de groupes restreints à partir d’un jeton d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="20547-104">The **RestrictedGroupSids** element represents a collection of restricted groups from a user's token.</span></span> 
  
```xml
<RestrictedGroupSids>
   <RestrictedGroupIdentifier/>
</RestrictedGroupSids>
```

 <span data-ttu-id="20547-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="20547-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20547-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="20547-106">Attributes and elements</span></span>

<span data-ttu-id="20547-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="20547-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20547-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="20547-108">Attributes</span></span>

<span data-ttu-id="20547-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="20547-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20547-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="20547-110">Child elements</span></span>

|<span data-ttu-id="20547-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20547-111">**Element**</span></span>|<span data-ttu-id="20547-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="20547-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20547-113">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="20547-113">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="20547-114">Représente l’identificateur de sécurité (SID) de groupe et les attributs d’un groupe restreint.</span><span class="sxs-lookup"><span data-stu-id="20547-114">Represents the group security identifier (SID) and attributes for a restricted group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20547-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="20547-115">Parent elements</span></span>

|<span data-ttu-id="20547-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20547-116">**Element**</span></span>|<span data-ttu-id="20547-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="20547-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20547-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="20547-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="20547-119">Utilisé dans l’en-tête SOAP pour sérialisation de jeton de l’authentification de serveur à serveur.</span><span class="sxs-lookup"><span data-stu-id="20547-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span> <span data-ttu-id="20547-120">Sérialisation de jeton n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="20547-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="20547-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="20547-121">Remarks</span></span>

<span data-ttu-id="20547-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="20547-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20547-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="20547-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20547-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="20547-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="20547-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="20547-125">Schema Name</span></span>  <br/> |<span data-ttu-id="20547-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="20547-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="20547-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="20547-127">Validation File</span></span>  <br/> |<span data-ttu-id="20547-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="20547-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="20547-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="20547-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="20547-130">False</span><span class="sxs-lookup"><span data-stu-id="20547-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20547-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="20547-131">See also</span></span>



- [<span data-ttu-id="20547-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="20547-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

