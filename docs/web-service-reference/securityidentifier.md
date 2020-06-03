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
description: L’élément SecurityIdentifier représente la forme SDDL (Security Descriptor Definition Language) d’un identificateur de sécurité (SID).
ms.openlocfilehash: c55e4a7f7f0b8f8a40e6fcaf8d18e253a6da2679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468802"
---
# <a name="securityidentifier"></a><span data-ttu-id="354d1-103">SecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="354d1-103">SecurityIdentifier</span></span>

<span data-ttu-id="354d1-104">L’élément **SecurityIdentifier** représente la forme SDDL (Security Descriptor Definition Language) d’un identificateur de sécurité ( [sid](sid.md)).</span><span class="sxs-lookup"><span data-stu-id="354d1-104">The **SecurityIdentifier** element represents the security descriptor definition language (SDDL) form of a security identifier ( [SID](sid.md)).</span></span>
  
```xml
<SecurityIdentifier/>
```

 <span data-ttu-id="354d1-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="354d1-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="354d1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="354d1-106">Attributes and elements</span></span>

<span data-ttu-id="354d1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="354d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="354d1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="354d1-108">Attributes</span></span>

<span data-ttu-id="354d1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="354d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="354d1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="354d1-110">Child elements</span></span>

<span data-ttu-id="354d1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="354d1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="354d1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="354d1-112">Parent elements</span></span>

|<span data-ttu-id="354d1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="354d1-113">**Element**</span></span>|<span data-ttu-id="354d1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="354d1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="354d1-115">GroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="354d1-115">GroupIdentifier</span></span>](groupidentifier.md) <br/> |<span data-ttu-id="354d1-116">Représente un identificateur et un attribut de sécurité unique pour un groupe d’objets Active Directory dont le compte est membre.</span><span class="sxs-lookup"><span data-stu-id="354d1-116">Represents a single security identifier and attribute for an Active Directory object group of which the account is a member.</span></span>  <br/> <span data-ttu-id="354d1-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="354d1-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[<span data-ttu-id="354d1-118">RestrictedGroupIdentifier</span><span class="sxs-lookup"><span data-stu-id="354d1-118">RestrictedGroupIdentifier</span></span>](restrictedgroupidentifier.md) <br/> |<span data-ttu-id="354d1-119">Représente l’identificateur de sécurité de groupe et les attributs d’un groupe restreint au sein d’un jeton utilisateur.</span><span class="sxs-lookup"><span data-stu-id="354d1-119">Represents the group security identifier and attributes for a restricted group within a user token.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="354d1-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="354d1-120">Remarks</span></span>

<span data-ttu-id="354d1-121">Cet élément est utilisé dans l’en-tête SOAP (Simple Object Access Protocol).</span><span class="sxs-lookup"><span data-stu-id="354d1-121">This element is used in the Simple Object Access Protocol (SOAP) header.</span></span>
  
<span data-ttu-id="354d1-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="354d1-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="354d1-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="354d1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="354d1-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="354d1-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="354d1-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="354d1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="354d1-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="354d1-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="354d1-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="354d1-127">Validation File</span></span>  <br/> |<span data-ttu-id="354d1-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="354d1-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="354d1-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="354d1-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="354d1-130">False</span><span class="sxs-lookup"><span data-stu-id="354d1-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="354d1-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="354d1-131">See also</span></span>



- [<span data-ttu-id="354d1-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="354d1-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

