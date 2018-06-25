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
description: L’élément SID représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité (SID) pour le compte à utiliser pour l’emprunt d’identité ou l’accès délégué.
ms.openlocfilehash: efcea42c12ec1d26ea31fdb8de337c37a2338a96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829492"
---
# <a name="sid"></a><span data-ttu-id="3cf49-103">SID</span><span class="sxs-lookup"><span data-stu-id="3cf49-103">SID</span></span>

<span data-ttu-id="3cf49-104">L’élément **SID** représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité (SID) pour le compte à utiliser pour l’emprunt d’identité ou l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="3cf49-104">The **SID** element represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation or delegate access.</span></span> 
  
```xml
<SID/>
```

 <span data-ttu-id="3cf49-105">**SIDType**</span><span class="sxs-lookup"><span data-stu-id="3cf49-105">**SIDType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3cf49-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3cf49-106">Attributes and elements</span></span>

<span data-ttu-id="3cf49-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3cf49-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3cf49-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3cf49-108">Attributes</span></span>

<span data-ttu-id="3cf49-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3cf49-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3cf49-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3cf49-110">Child elements</span></span>

<span data-ttu-id="3cf49-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3cf49-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3cf49-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3cf49-112">Parent elements</span></span>

|<span data-ttu-id="3cf49-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3cf49-113">**Element**</span></span>|<span data-ttu-id="3cf49-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3cf49-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3cf49-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="3cf49-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="3cf49-116">Représente un compte pour emprunter l’identité lors de l’utilisation de l’en-tête SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="3cf49-116">Represents an account to impersonate when using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="3cf49-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="3cf49-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="3cf49-118">Nom d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="3cf49-118">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="3cf49-119">Identifie un utilisateur délégué ou un utilisateur disposant des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="3cf49-119">Identifies a delegate user or a user with folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3cf49-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3cf49-120">Text value</span></span>

<span data-ttu-id="3cf49-121">La valeur de texte est une représentation de chaîne d’un identificateur de sécurité.</span><span class="sxs-lookup"><span data-stu-id="3cf49-121">The text value is a string representation of a SID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3cf49-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="3cf49-122">Remarks</span></span>

<span data-ttu-id="3cf49-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="3cf49-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3cf49-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3cf49-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3cf49-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3cf49-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3cf49-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3cf49-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3cf49-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3cf49-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="3cf49-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3cf49-128">Validation File</span></span>  <br/> |<span data-ttu-id="3cf49-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3cf49-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3cf49-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3cf49-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3cf49-131">False</span><span class="sxs-lookup"><span data-stu-id="3cf49-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3cf49-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3cf49-132">See also</span></span>



- [<span data-ttu-id="3cf49-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3cf49-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

