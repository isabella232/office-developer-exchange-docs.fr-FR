---
title: PrincipalName
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
description: L’élément PrincipalName représente le nom d’utilisateur principal (UPN) du compte à utiliser pour l’emprunt d’identité Exchange.
ms.openlocfilehash: 31412c1461264e28bf8d52c957a457e8d1e847ef
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44440189"
---
# <a name="principalname"></a><span data-ttu-id="38cb4-103">PrincipalName</span><span class="sxs-lookup"><span data-stu-id="38cb4-103">PrincipalName</span></span>

<span data-ttu-id="38cb4-104">L’élément **PrincipalName** représente le nom d’utilisateur principal (UPN) du compte à utiliser pour l’emprunt d’identité Exchange.</span><span class="sxs-lookup"><span data-stu-id="38cb4-104">The **PrincipalName** element represents the user principal name (UPN) of the account to be used for Exchange impersonation.</span></span> 
  
```xml
<PrincipalName/>
```

 <span data-ttu-id="38cb4-105">**PrincipalNameType**</span><span class="sxs-lookup"><span data-stu-id="38cb4-105">**PrincipalNameType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38cb4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="38cb4-106">Attributes and elements</span></span>

<span data-ttu-id="38cb4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="38cb4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38cb4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="38cb4-108">Attributes</span></span>

<span data-ttu-id="38cb4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="38cb4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38cb4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="38cb4-110">Child elements</span></span>

<span data-ttu-id="38cb4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="38cb4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38cb4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="38cb4-112">Parent elements</span></span>

|<span data-ttu-id="38cb4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="38cb4-113">**Element**</span></span>|<span data-ttu-id="38cb4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="38cb4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38cb4-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="38cb4-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="38cb4-116">Représente un compte dont l’identité est empruntée lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="38cb4-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="38cb4-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="38cb4-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38cb4-118">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="38cb4-118">Text value</span></span>

<span data-ttu-id="38cb4-119">La valeur de texte représente le nom d’utilisateur principal d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="38cb4-119">The text value represents the UPN of a user.</span></span> <span data-ttu-id="38cb4-120">Cette valeur existe sur l’objet utilisateur dans le service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="38cb4-120">This value exists on the user object in the Active Directory directory service.</span></span> <span data-ttu-id="38cb4-121">Il contient le nom d’ouverture de session de l’utilisateur et un nom de domaine qui identifie le domaine dans lequel se trouve le compte d’utilisateur, au format suivant : `someone@example.com` .</span><span class="sxs-lookup"><span data-stu-id="38cb4-121">This contains the user logon name and a domain name that identifies the domain in which the user account is located, in the following format:  `someone@example.com`.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="38cb4-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="38cb4-122">Remarks</span></span>

<span data-ttu-id="38cb4-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="38cb4-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38cb4-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="38cb4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38cb4-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="38cb4-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38cb4-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="38cb4-126">Schema Name</span></span>  <br/> |<span data-ttu-id="38cb4-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="38cb4-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="38cb4-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="38cb4-128">Validation File</span></span>  <br/> |<span data-ttu-id="38cb4-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="38cb4-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="38cb4-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="38cb4-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="38cb4-131">False</span><span class="sxs-lookup"><span data-stu-id="38cb4-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38cb4-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="38cb4-132">See also</span></span>



- [<span data-ttu-id="38cb4-133">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38cb4-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="38cb4-134">Autorisation de serveur à serveur dans EWS</span><span class="sxs-lookup"><span data-stu-id="38cb4-134">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

