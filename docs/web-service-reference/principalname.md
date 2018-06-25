---
title: Au PrincipalName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrincipalName
api_type:
- schema
ms.assetid: 88c142d4-0bc7-43ea-a997-d7200664d900
description: L’élément au PrincipalName représente le nom d’utilisateur principal (UPN) du compte à utiliser pour l’emprunt d’identité Exchange.
ms.openlocfilehash: d8557ce0435a11a5602372517db1f576028a9c97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828882"
---
# <a name="principalname"></a><span data-ttu-id="97dfb-103">Au PrincipalName</span><span class="sxs-lookup"><span data-stu-id="97dfb-103">PrincipalName</span></span>

<span data-ttu-id="97dfb-104">L’élément **au PrincipalName** représente le nom d’utilisateur principal (UPN) du compte à utiliser pour l’emprunt d’identité Exchange.</span><span class="sxs-lookup"><span data-stu-id="97dfb-104">The **PrincipalName** element represents the user principal name (UPN) of the account to be used for Exchange impersonation.</span></span> 
  
```xml
<PrincipalName/>
```

 <span data-ttu-id="97dfb-105">**PrincipalNameType**</span><span class="sxs-lookup"><span data-stu-id="97dfb-105">**PrincipalNameType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97dfb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="97dfb-106">Attributes and elements</span></span>

<span data-ttu-id="97dfb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="97dfb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97dfb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="97dfb-108">Attributes</span></span>

<span data-ttu-id="97dfb-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="97dfb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97dfb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="97dfb-110">Child elements</span></span>

<span data-ttu-id="97dfb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="97dfb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="97dfb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="97dfb-112">Parent elements</span></span>

|<span data-ttu-id="97dfb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="97dfb-113">**Element**</span></span>|<span data-ttu-id="97dfb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="97dfb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97dfb-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="97dfb-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="97dfb-116">Représente un compte pour emprunter l’identité lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="97dfb-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="97dfb-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="97dfb-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="97dfb-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="97dfb-118">Text value</span></span>

<span data-ttu-id="97dfb-119">La valeur de text représente l’UPN d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="97dfb-119">The text value represents the UPN of a user.</span></span> <span data-ttu-id="97dfb-120">Cette valeur existe sur l’objet utilisateur dans le service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="97dfb-120">This value exists on the user object in the Active Directory directory service.</span></span> <span data-ttu-id="97dfb-121">Contient le nom d’utilisateur et un nom de domaine qui identifie le domaine dans lequel le compte d’utilisateur se trouve, dans le format suivant : `someone@example.com`.</span><span class="sxs-lookup"><span data-stu-id="97dfb-121">This contains the user logon name and a domain name that identifies the domain in which the user account is located, in the following format:  `someone@example.com`.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="97dfb-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="97dfb-122">Remarks</span></span>

<span data-ttu-id="97dfb-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="97dfb-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97dfb-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="97dfb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97dfb-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="97dfb-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97dfb-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="97dfb-126">Schema Name</span></span>  <br/> |<span data-ttu-id="97dfb-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="97dfb-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="97dfb-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="97dfb-128">Validation File</span></span>  <br/> |<span data-ttu-id="97dfb-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="97dfb-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97dfb-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="97dfb-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="97dfb-131">False</span><span class="sxs-lookup"><span data-stu-id="97dfb-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97dfb-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="97dfb-132">See also</span></span>



- [<span data-ttu-id="97dfb-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="97dfb-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="97dfb-134">Autorisation de serveur à serveur dans EWS</span><span class="sxs-lookup"><span data-stu-id="97dfb-134">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

