---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: L’élément ConnectingSID représente un compte pour emprunter l’identité lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.
ms.openlocfilehash: 6e0bb90e197ce22bcd982a6d51954a88f3a2cf03
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755546"
---
# <a name="connectingsid"></a><span data-ttu-id="e9543-103">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="e9543-103">ConnectingSID</span></span>

<span data-ttu-id="e9543-104">L’élément **ConnectingSID** représente un compte pour emprunter l’identité lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="e9543-104">The **ConnectingSID** element represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span> 
  
[<span data-ttu-id="e9543-105">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="e9543-105">ExchangeImpersonation</span></span>](exchangeimpersonation.md)
  
[<span data-ttu-id="e9543-106">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="e9543-106">ConnectingSID</span></span>](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

 <span data-ttu-id="e9543-107">**ConnectingSIDType**</span><span class="sxs-lookup"><span data-stu-id="e9543-107">**ConnectingSIDType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9543-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e9543-108">Attributes and elements</span></span>

<span data-ttu-id="e9543-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e9543-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9543-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="e9543-110">Attributes</span></span>

<span data-ttu-id="e9543-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e9543-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9543-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e9543-112">Child elements</span></span>

|<span data-ttu-id="e9543-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9543-113">**Element**</span></span>|<span data-ttu-id="e9543-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9543-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9543-115">Au PrincipalName</span><span class="sxs-lookup"><span data-stu-id="e9543-115">PrincipalName</span></span>](principalname.md) <br/> |<span data-ttu-id="e9543-116">Représente le nom d’utilisateur principal (UPN) du compte à utiliser pour l’emprunt d’identité.</span><span class="sxs-lookup"><span data-stu-id="e9543-116">Represents the user principal name (UPN) of the account to use for impersonation.</span></span> <span data-ttu-id="e9543-117">Il doit s’agir de l’UPN pour le domaine où le compte d’utilisateur existe.</span><span class="sxs-lookup"><span data-stu-id="e9543-117">This should be the UPN for the domain where the user account exists.</span></span>  <br/> |
|[<span data-ttu-id="e9543-118">SID</span><span class="sxs-lookup"><span data-stu-id="e9543-118">SID</span></span>](sid.md) <br/> |<span data-ttu-id="e9543-119">Représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité (SID) pour le compte à utiliser pour l’emprunt d’identité.</span><span class="sxs-lookup"><span data-stu-id="e9543-119">Represents the security descriptor definition language (SDDL) form of the security identifier (SID) for the account to use for impersonation.</span></span>  <br/> |
|[<span data-ttu-id="e9543-120">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="e9543-120">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="e9543-121">Représente l’adresse SMTP Simple Mail Transfer Protocol () principal du compte à utiliser pour l’emprunt d’identité Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9543-121">Represents the primary Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange impersonation.</span></span> <span data-ttu-id="e9543-122">Si l’adresse SMTP principale est fourni, une recherche de service d’annuaire Active Directory supplémentaire seront coût afin d’obtenir le SID de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e9543-122">If the primary SMTP address is supplied, it will cost an extra Active Directory directory service lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="e9543-123">Nous vous recommandons d’utiliser le SID ou UPN si elles sont disponibles.</span><span class="sxs-lookup"><span data-stu-id="e9543-123">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
|[<span data-ttu-id="e9543-124">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="e9543-124">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="e9543-125">Représente l’adresse SMTP Simple Mail Transfer Protocol () du compte à utiliser pour l’emprunt d’identité Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9543-125">Represents the Simple Mail Transfer Protocol (SMTP) address of the account to use for Exchange Impersonation.</span></span> <span data-ttu-id="e9543-126">Si l’adresse SMTP est fourni, une recherche Active Directory supplémentaire seront coût afin d’obtenir le SID de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e9543-126">If the SMTP address is supplied, it will cost an extra Active Directory lookup in order to obtain the SID of the user.</span></span> <span data-ttu-id="e9543-127">Nous vous recommandons d’utiliser le SID ou UPN si elles sont disponibles.</span><span class="sxs-lookup"><span data-stu-id="e9543-127">We recommend that you use the SID or UPN if they are available.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9543-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e9543-128">Parent elements</span></span>

|<span data-ttu-id="e9543-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9543-129">**Element**</span></span>|<span data-ttu-id="e9543-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9543-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9543-131">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="e9543-131">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="e9543-132">Utilisé dans l’en-tête SOAP d’une demande.</span><span class="sxs-lookup"><span data-stu-id="e9543-132">Used in the SOAP header of a request.</span></span> <span data-ttu-id="e9543-133">Lorsque cet élément est présent, l’appelant essaie d’emprunter l’identité du compte qui est contenu dans l’élément **ExchangeImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="e9543-133">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span>  <br/> <span data-ttu-id="e9543-134">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="e9543-134">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9543-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="e9543-135">Remarks</span></span>

<span data-ttu-id="e9543-136">Le compte d’appel doit avoir **ms-exch-l’emprunt d’identité** sur le serveur d’accès au Client et le **ms-exch-MayImpersonate** droite sur soit la base de données de boîtes aux lettres contenant la boîte aux lettres pour emprunter l’identité ou l’utilisateur Active Directory ou un contact objet.</span><span class="sxs-lookup"><span data-stu-id="e9543-136">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory user or contact object.</span></span> 
  
<span data-ttu-id="e9543-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e9543-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9543-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e9543-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9543-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e9543-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9543-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e9543-140">Schema name</span></span>  <br/> |<span data-ttu-id="e9543-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e9543-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9543-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e9543-142">Validation file</span></span>  <br/> |<span data-ttu-id="e9543-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e9543-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9543-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e9543-144">Can be empty</span></span>  <br/> |<span data-ttu-id="e9543-145">False</span><span class="sxs-lookup"><span data-stu-id="e9543-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9543-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e9543-146">See also</span></span>



[<span data-ttu-id="e9543-147">Autorisation de serveur à serveur dans EWS</span><span class="sxs-lookup"><span data-stu-id="e9543-147">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
