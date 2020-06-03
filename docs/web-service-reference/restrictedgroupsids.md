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
description: L’élément RestrictedGroupSids représente une collection de groupes restreints à partir du jeton d’un utilisateur.
ms.openlocfilehash: 739a73d2ac4bdbbee03650d035271b5c8d9ea25a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465358"
---
# <a name="restrictedgroupsids"></a><span data-ttu-id="7878f-103">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="7878f-103">RestrictedGroupSids</span></span>

<span data-ttu-id="7878f-104">L’élément **RestrictedGroupSids** représente une collection de groupes restreints à partir du jeton d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7878f-104">The **RestrictedGroupSids** element represents a collection of restricted groups from a user's token.</span></span> 
  
```xml
<RestrictedGroupSids>
   <RestrictedGroupIdentifier/>
</RestrictedGroupSids>
```

 <span data-ttu-id="7878f-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="7878f-105">**NonEmptyArrayOfRestrictedGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7878f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7878f-106">Attributes and elements</span></span>

<span data-ttu-id="7878f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7878f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7878f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7878f-108">Attributes</span></span>

<span data-ttu-id="7878f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7878f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7878f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7878f-110">Child elements</span></span>

|<span data-ttu-id="7878f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7878f-111">**Element**</span></span>|<span data-ttu-id="7878f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7878f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7878f-113">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="7878f-113">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="7878f-114">Représente l’identificateur de sécurité (SID) de groupe et les attributs d’un groupe restreint.</span><span class="sxs-lookup"><span data-stu-id="7878f-114">Represents the group security identifier (SID) and attributes for a restricted group.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7878f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7878f-115">Parent elements</span></span>

|<span data-ttu-id="7878f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7878f-116">**Element**</span></span>|<span data-ttu-id="7878f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7878f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7878f-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="7878f-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="7878f-119">Utilisé dans l’en-tête SOAP pour la sérialisation de jetons dans l’authentification de serveur à serveur.</span><span class="sxs-lookup"><span data-stu-id="7878f-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span> <span data-ttu-id="7878f-120">La sérialisation de jetons n’est pas prise en charge.</span><span class="sxs-lookup"><span data-stu-id="7878f-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7878f-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="7878f-121">Remarks</span></span>

<span data-ttu-id="7878f-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7878f-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7878f-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7878f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7878f-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7878f-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7878f-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7878f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7878f-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7878f-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="7878f-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7878f-127">Validation File</span></span>  <br/> |<span data-ttu-id="7878f-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7878f-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7878f-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7878f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="7878f-130">False</span><span class="sxs-lookup"><span data-stu-id="7878f-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7878f-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7878f-131">See also</span></span>



- [<span data-ttu-id="7878f-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7878f-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

