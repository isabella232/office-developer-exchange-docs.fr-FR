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
description: L’élément GroupSids représente une collection d’identificateurs de sécurité d’objet de groupe de service d’annuaire Active Directory.
ms.openlocfilehash: 40f36176fcaa3e2160237f269fb2dc3b12bf8af2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530063"
---
# <a name="groupsids"></a><span data-ttu-id="c50fd-103">GroupSids</span><span class="sxs-lookup"><span data-stu-id="c50fd-103">GroupSids</span></span>

<span data-ttu-id="c50fd-104">L’élément **GroupSids** représente une collection d’identificateurs de sécurité d’objet de groupe de service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c50fd-104">The **GroupSids** element represents a collection of Active Directory directory service group object security identifiers.</span></span> 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 <span data-ttu-id="c50fd-105">**NonEmptyArrayOfGroupIdentifiersType**</span><span class="sxs-lookup"><span data-stu-id="c50fd-105">**NonEmptyArrayOfGroupIdentifiersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c50fd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c50fd-106">Attributes and elements</span></span>

<span data-ttu-id="c50fd-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c50fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c50fd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c50fd-108">Attributes</span></span>

<span data-ttu-id="c50fd-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c50fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c50fd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c50fd-110">Child elements</span></span>

|<span data-ttu-id="c50fd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c50fd-111">**Element**</span></span>|<span data-ttu-id="c50fd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c50fd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c50fd-113">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="c50fd-113">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="c50fd-114">Représente un identificateur et un attribut de sécurité unique pour un groupe d’objets Active Directory dont le compte est membre.</span><span class="sxs-lookup"><span data-stu-id="c50fd-114">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c50fd-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c50fd-115">Parent elements</span></span>

|<span data-ttu-id="c50fd-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c50fd-116">**Element**</span></span>|<span data-ttu-id="c50fd-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c50fd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c50fd-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="c50fd-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="c50fd-119">Utilisé dans l’en-tête SOAP (Simple Object Access Protocol) pour la sérialisation des jetons dans l’authentification de serveur à serveur.</span><span class="sxs-lookup"><span data-stu-id="c50fd-119">Used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="c50fd-120">La sérialisation de jetons n’est pas prise en charge.</span><span class="sxs-lookup"><span data-stu-id="c50fd-120">Token serialization is not supported.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c50fd-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="c50fd-121">Remarks</span></span>

<span data-ttu-id="c50fd-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c50fd-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c50fd-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c50fd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c50fd-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c50fd-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c50fd-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c50fd-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c50fd-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c50fd-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="c50fd-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c50fd-127">Validation File</span></span>  <br/> |<span data-ttu-id="c50fd-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c50fd-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c50fd-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c50fd-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c50fd-130">False</span><span class="sxs-lookup"><span data-stu-id="c50fd-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c50fd-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c50fd-131">See also</span></span>



- [<span data-ttu-id="c50fd-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c50fd-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

