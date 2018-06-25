---
title: ExchangeImpersonation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExchangeImpersonation
api_type:
- schema
ms.assetid: d8cbac49-47d0-4745-a2a7-545d33f8da93
description: L’élément ExchangeImpersonation est utilisé dans l’en-tête SOAP d’une demande. Lorsque cet élément est présent, l’appelant essaie d’emprunter l’identité du compte qui est contenu dans l’élément ExchangeImpersonation.
ms.openlocfilehash: aedeff22cda865ce1eec80dab9760d49fdc178f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756241"
---
# <a name="exchangeimpersonation"></a><span data-ttu-id="cda11-104">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="cda11-104">ExchangeImpersonation</span></span>

<span data-ttu-id="cda11-105">L’élément **ExchangeImpersonation** est utilisé dans l’en-tête SOAP d’une demande.</span><span class="sxs-lookup"><span data-stu-id="cda11-105">The **ExchangeImpersonation** element is used in the SOAP header of a request.</span></span> <span data-ttu-id="cda11-106">Lorsque cet élément est présent, l’appelant essaie d’emprunter l’identité du compte qui est contenu dans l’élément **ExchangeImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="cda11-106">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span> 
  
[<span data-ttu-id="cda11-107">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="cda11-107">ExchangeImpersonation</span></span>](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 <span data-ttu-id="cda11-108">**ExchangeImpersonationType**</span><span class="sxs-lookup"><span data-stu-id="cda11-108">**ExchangeImpersonationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cda11-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cda11-109">Attributes and elements</span></span>

<span data-ttu-id="cda11-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cda11-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cda11-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="cda11-111">Attributes</span></span>

<span data-ttu-id="cda11-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cda11-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cda11-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cda11-113">Child elements</span></span>

|<span data-ttu-id="cda11-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cda11-114">**Element**</span></span>|<span data-ttu-id="cda11-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="cda11-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cda11-116">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="cda11-116">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="cda11-117">Représente un compte pour emprunter l’identité lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="cda11-117">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cda11-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cda11-118">Parent elements</span></span>

<span data-ttu-id="cda11-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cda11-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cda11-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="cda11-120">Remarks</span></span>

<span data-ttu-id="cda11-121">Le compte d’appel doit avoir **ms-exch-l’emprunt d’identité** sur le serveur d’accès au Client et le **ms-exch-MayImpersonate** droit soit utilisateur/Contact de l’Active Directory ou de la base de données de boîtes aux lettres contenant la boîte aux lettres pour emprunter l’identité objet.</span><span class="sxs-lookup"><span data-stu-id="cda11-121">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory User/Contact object.</span></span> 
  
<span data-ttu-id="cda11-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="cda11-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cda11-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cda11-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cda11-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cda11-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cda11-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cda11-125">Schema name</span></span>  <br/> |<span data-ttu-id="cda11-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cda11-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="cda11-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cda11-127">Validation file</span></span>  <br/> |<span data-ttu-id="cda11-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cda11-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cda11-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cda11-129">Can be empty</span></span>  <br/> |<span data-ttu-id="cda11-130">False</span><span class="sxs-lookup"><span data-stu-id="cda11-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cda11-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cda11-131">See also</span></span>



[<span data-ttu-id="cda11-132">Autorisation de serveur à serveur dans EWS</span><span class="sxs-lookup"><span data-stu-id="cda11-132">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

