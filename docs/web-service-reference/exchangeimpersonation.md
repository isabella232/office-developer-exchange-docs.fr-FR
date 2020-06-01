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
description: L’élément ExchangeImpersonation est utilisé dans l’en-tête SOAP d’une demande. Lorsque cet élément est présent, l’appelant tente d’emprunter l’identité du compte qui est contenu dans l’élément ExchangeImpersonation.
ms.openlocfilehash: 188219d95453dc45378c6ca65ab93c2de7db4eac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463348"
---
# <a name="exchangeimpersonation"></a><span data-ttu-id="79090-104">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="79090-104">ExchangeImpersonation</span></span>

<span data-ttu-id="79090-105">L’élément **ExchangeImpersonation** est utilisé dans l’en-tête SOAP d’une demande.</span><span class="sxs-lookup"><span data-stu-id="79090-105">The **ExchangeImpersonation** element is used in the SOAP header of a request.</span></span> <span data-ttu-id="79090-106">Lorsque cet élément est présent, l’appelant tente d’emprunter l’identité du compte qui est contenu dans l’élément **ExchangeImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="79090-106">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span> 
  
[<span data-ttu-id="79090-107">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="79090-107">ExchangeImpersonation</span></span>](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 <span data-ttu-id="79090-108">**ExchangeImpersonationType**</span><span class="sxs-lookup"><span data-stu-id="79090-108">**ExchangeImpersonationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79090-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="79090-109">Attributes and elements</span></span>

<span data-ttu-id="79090-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="79090-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79090-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="79090-111">Attributes</span></span>

<span data-ttu-id="79090-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="79090-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79090-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="79090-113">Child elements</span></span>

|<span data-ttu-id="79090-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79090-114">**Element**</span></span>|<span data-ttu-id="79090-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="79090-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79090-116">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="79090-116">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="79090-117">Représente un compte dont l’identité est empruntée lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="79090-117">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="79090-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="79090-118">Parent elements</span></span>

<span data-ttu-id="79090-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79090-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79090-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="79090-120">Remarks</span></span>

<span data-ttu-id="79090-121">Le compte appelant doit disposer du droit **ms-Exch-emprunt d’identité** sur le serveur d’accès au client et du droit **ms-Exch-MayImpersonate** sur la base de données de boîtes aux lettres qui contient la boîte aux lettres à emprunter l’identité ou l’objet utilisateur/contact Active Directory.</span><span class="sxs-lookup"><span data-stu-id="79090-121">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory User/Contact object.</span></span> 
  
<span data-ttu-id="79090-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="79090-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79090-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="79090-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79090-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="79090-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79090-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="79090-125">Schema name</span></span>  <br/> |<span data-ttu-id="79090-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="79090-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="79090-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="79090-127">Validation file</span></span>  <br/> |<span data-ttu-id="79090-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="79090-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79090-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="79090-129">Can be empty</span></span>  <br/> |<span data-ttu-id="79090-130">False</span><span class="sxs-lookup"><span data-stu-id="79090-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79090-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79090-131">See also</span></span>



[<span data-ttu-id="79090-132">Autorisation de serveur à serveur dans EWS</span><span class="sxs-lookup"><span data-stu-id="79090-132">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

