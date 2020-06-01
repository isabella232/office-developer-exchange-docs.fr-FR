---
title: SID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SID
api_type:
- schema
ms.assetid: 2f33b29b-163b-4106-a74d-6fb76ec38951
description: L’élément SID représente la forme SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité (SID) du compte à utiliser pour l’emprunt d’identité ou l’accès délégué.
ms.openlocfilehash: 0e3f740e9a056f7c0042049d97757b5f2d3c441d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468046"
---
# <a name="sid"></a><span data-ttu-id="12e54-103">SID</span><span class="sxs-lookup"><span data-stu-id="12e54-103">SID</span></span>

<span data-ttu-id="12e54-104">L’élément **sid** représente la forme SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité (SID) du compte à utiliser pour l’emprunt d’identité ou l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="12e54-104">The **SID** element represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation or delegate access.</span></span> 
  
```xml
<SID/>
```

 <span data-ttu-id="12e54-105">**SIDType**</span><span class="sxs-lookup"><span data-stu-id="12e54-105">**SIDType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12e54-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="12e54-106">Attributes and elements</span></span>

<span data-ttu-id="12e54-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="12e54-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12e54-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="12e54-108">Attributes</span></span>

<span data-ttu-id="12e54-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="12e54-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12e54-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="12e54-110">Child elements</span></span>

<span data-ttu-id="12e54-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="12e54-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12e54-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="12e54-112">Parent elements</span></span>

|<span data-ttu-id="12e54-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="12e54-113">**Element**</span></span>|<span data-ttu-id="12e54-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="12e54-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12e54-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="12e54-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="12e54-116">Représente un compte dont l’identité est empruntée lors de l’utilisation de l’en-tête SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="12e54-116">Represents an account to impersonate when using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="12e54-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="12e54-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="12e54-118">UserId</span><span class="sxs-lookup"><span data-stu-id="12e54-118">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="12e54-119">Identifie un utilisateur délégué ou un utilisateur disposant des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="12e54-119">Identifies a delegate user or a user with folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12e54-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="12e54-120">Text value</span></span>

<span data-ttu-id="12e54-121">La valeur de texte est une représentation sous forme de chaîne d’un SID.</span><span class="sxs-lookup"><span data-stu-id="12e54-121">The text value is a string representation of a SID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="12e54-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="12e54-122">Remarks</span></span>

<span data-ttu-id="12e54-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="12e54-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12e54-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="12e54-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12e54-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="12e54-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12e54-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="12e54-126">Schema Name</span></span>  <br/> |<span data-ttu-id="12e54-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="12e54-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="12e54-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="12e54-128">Validation File</span></span>  <br/> |<span data-ttu-id="12e54-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="12e54-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12e54-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="12e54-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="12e54-131">False</span><span class="sxs-lookup"><span data-stu-id="12e54-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12e54-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="12e54-132">See also</span></span>



- [<span data-ttu-id="12e54-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="12e54-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

