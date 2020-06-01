---
title: PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: L’élément PrimarySmtpAddress représente l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un compte à utiliser pour l’autorisation de serveur à serveur ou l’accès délégué.
ms.openlocfilehash: eea995b3e546d7e94e65cf9b230b639a781c4928
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467962"
---
# <a name="primarysmtpaddress"></a><span data-ttu-id="ddbca-103">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="ddbca-103">PrimarySmtpAddress</span></span>

<span data-ttu-id="ddbca-104">L’élément **PrimarySmtpAddress** représente l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un compte à utiliser pour l’autorisation de serveur à serveur ou l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="ddbca-104">The **PrimarySmtpAddress** element represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization or delegate access.</span></span> 
  
```xml
<PrimarySmtpAddress/>
```

 <span data-ttu-id="ddbca-105">**PrimarySmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="ddbca-105">**PrimarySmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ddbca-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ddbca-106">Attributes and elements</span></span>

<span data-ttu-id="ddbca-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ddbca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ddbca-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ddbca-108">Attributes</span></span>

<span data-ttu-id="ddbca-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ddbca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ddbca-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ddbca-110">Child elements</span></span>

<span data-ttu-id="ddbca-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ddbca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ddbca-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ddbca-112">Parent elements</span></span>

|<span data-ttu-id="ddbca-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ddbca-113">**Element**</span></span>|<span data-ttu-id="ddbca-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ddbca-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddbca-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="ddbca-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="ddbca-116">Représente un compte dont l’identité est empruntée lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="ddbca-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="ddbca-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="ddbca-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="ddbca-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="ddbca-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="ddbca-119">Utilisé dans l’en-tête SOAP pour la sérialisation de jetons dans l’authentification de serveur à serveur.</span><span class="sxs-lookup"><span data-stu-id="ddbca-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span>  <br/> |
|[<span data-ttu-id="ddbca-120">UserId</span><span class="sxs-lookup"><span data-stu-id="ddbca-120">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="ddbca-121">Identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="ddbca-121">Identifies a delegate user or a user who has folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ddbca-122">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ddbca-122">Text value</span></span>

<span data-ttu-id="ddbca-123">Une valeur de texte qui représente une adresse SMTP est requise.</span><span class="sxs-lookup"><span data-stu-id="ddbca-123">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ddbca-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="ddbca-124">Remarks</span></span>

<span data-ttu-id="ddbca-125">Les services Web Exchange requièrent que les boîtes aux lettres soient identifiées par l’adresse SMTP principale de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ddbca-125">Exchange Web Services requires that mailboxes be identified by the primary SMTP address of the mailbox.</span></span> <span data-ttu-id="ddbca-126">Les adresses proxy ou alternatives ne sont pas acceptées.</span><span class="sxs-lookup"><span data-stu-id="ddbca-126">Proxy or alternative addresses are not accepted.</span></span>
  
<span data-ttu-id="ddbca-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ddbca-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ddbca-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ddbca-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ddbca-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ddbca-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ddbca-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ddbca-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ddbca-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ddbca-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ddbca-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ddbca-132">Validation File</span></span>  <br/> |<span data-ttu-id="ddbca-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ddbca-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ddbca-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ddbca-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ddbca-135">False</span><span class="sxs-lookup"><span data-stu-id="ddbca-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ddbca-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ddbca-136">See also</span></span>



- [<span data-ttu-id="ddbca-137">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ddbca-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ddbca-138">Autorisation de serveur à serveur dans EWS</span><span class="sxs-lookup"><span data-stu-id="ddbca-138">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[<span data-ttu-id="ddbca-139">Utilisation de l’accès délégué</span><span class="sxs-lookup"><span data-stu-id="ddbca-139">Working with Delegate Access</span></span>](https://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

