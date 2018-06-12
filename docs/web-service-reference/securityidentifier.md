---
title: SecurityIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SecurityIdentifier
api_type:
- schema
ms.assetid: f7656729-f2c9-41cc-b1ec-60f480fc4dab
description: L’élément SecurityIdentifier représente le formulaire sécurité descripteur definition language (SDDL) d’un identificateur de sécurité (SID).
ms.openlocfilehash: c18d7d4505c618792497c32c7499eab9ac82989e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829314"
---
# <a name="securityidentifier"></a><span data-ttu-id="05bd7-103">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="05bd7-103">SecurityIdentifier</span></span>

<span data-ttu-id="05bd7-104">L’élément **SecurityIdentifier** représente le formulaire sécurité descripteur definition language (SDDL) d’un identificateur de sécurité ( [SID](sid.md)).</span><span class="sxs-lookup"><span data-stu-id="05bd7-104">The **SecurityIdentifier** element represents the security descriptor definition language (SDDL) form of a security identifier ( [SID](sid.md)).</span></span>
  
```xml
<SecurityIdentifier/>
```

 <span data-ttu-id="05bd7-105">**string**</span><span class="sxs-lookup"><span data-stu-id="05bd7-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05bd7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="05bd7-106">Attributes and elements</span></span>

<span data-ttu-id="05bd7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="05bd7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05bd7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="05bd7-108">Attributes</span></span>

<span data-ttu-id="05bd7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05bd7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05bd7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="05bd7-110">Child elements</span></span>

<span data-ttu-id="05bd7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05bd7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05bd7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="05bd7-112">Parent elements</span></span>

|<span data-ttu-id="05bd7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05bd7-113">**Element**</span></span>|<span data-ttu-id="05bd7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="05bd7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05bd7-115">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="05bd7-115">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="05bd7-116">Représente un identificateur de sécurité unique et un attribut pour un groupe d’objets Active Directory dont le compte est membre.</span><span class="sxs-lookup"><span data-stu-id="05bd7-116">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> <span data-ttu-id="05bd7-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="05bd7-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[<span data-ttu-id="05bd7-118">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="05bd7-118">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="05bd7-119">Représente l’identificateur du groupe de sécurité et les attributs d’un groupe restreint au sein d’un jeton utilisateur.</span><span class="sxs-lookup"><span data-stu-id="05bd7-119">Represents the group security identifier and attributes for a restricted group within a user token.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="05bd7-120">Note</span><span class="sxs-lookup"><span data-stu-id="05bd7-120">Remarks</span></span>

<span data-ttu-id="05bd7-121">Cet élément est utilisé dans l’en-tête SOAP Simple Object Access Protocol ().</span><span class="sxs-lookup"><span data-stu-id="05bd7-121">This element is used in the Simple Object Access Protocol (SOAP) header.</span></span>
  
<span data-ttu-id="05bd7-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="05bd7-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05bd7-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="05bd7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05bd7-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="05bd7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05bd7-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="05bd7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="05bd7-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="05bd7-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="05bd7-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="05bd7-127">Validation File</span></span>  <br/> |<span data-ttu-id="05bd7-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05bd7-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05bd7-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="05bd7-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="05bd7-130">False</span><span class="sxs-lookup"><span data-stu-id="05bd7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05bd7-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05bd7-131">See also</span></span>



- [<span data-ttu-id="05bd7-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="05bd7-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

