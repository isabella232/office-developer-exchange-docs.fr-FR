---
title: EmailAddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20049467-c01a-4c7d-8ada-ca1801cc95ed
description: L’élément EmailAddressEntity spécifie une entité d’adresse de messagerie unique.
ms.openlocfilehash: c149ee69c1ed08c33d0341c8dfdac3bcda040afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756116"
---
# <a name="emailaddressentity"></a><span data-ttu-id="9954f-103">EmailAddressEntity</span><span class="sxs-lookup"><span data-stu-id="9954f-103">EmailAddressEntity</span></span>

<span data-ttu-id="9954f-104">L’élément **EmailAddressEntity** spécifie une entité d’adresse de messagerie unique.</span><span class="sxs-lookup"><span data-stu-id="9954f-104">The **EmailAddressEntity** element specifies a single email address entity.</span></span> 
  
```XML
<EmailAddressEntity>
    <EmailAddress></EmailAddress>
</EmailAddressEntity>
```

 <span data-ttu-id="9954f-105">**EmailAddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="9954f-105">**EmailAddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9954f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9954f-106">Attributes and elements</span></span>

<span data-ttu-id="9954f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9954f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9954f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9954f-108">Attributes</span></span>

<span data-ttu-id="9954f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9954f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9954f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9954f-110">Child elements</span></span>

|<span data-ttu-id="9954f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9954f-111">**Element**</span></span>|<span data-ttu-id="9954f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9954f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9954f-113">EmailAddress (chaîne)</span><span class="sxs-lookup"><span data-stu-id="9954f-113">EmailAddress (string)</span></span>](emailaddress-string.md) <br/> |<span data-ttu-id="9954f-114">Spécifie une adresse de messagerie unique.</span><span class="sxs-lookup"><span data-stu-id="9954f-114">Specifies a single email address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9954f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9954f-115">Parent elements</span></span>

|<span data-ttu-id="9954f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9954f-116">**Element**</span></span>|<span data-ttu-id="9954f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="9954f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9954f-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="9954f-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="9954f-119">Spécifie un tableau des entités d’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="9954f-119">Specifies an array of email address entities.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9954f-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="9954f-120">Remarks</span></span>

<span data-ttu-id="9954f-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9954f-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9954f-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9954f-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9954f-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9954f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9954f-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9954f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9954f-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9954f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9954f-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="9954f-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="9954f-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="9954f-127">Validation File</span></span>  <br/> |<span data-ttu-id="9954f-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="9954f-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9954f-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9954f-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9954f-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9954f-130">See also</span></span>



- [<span data-ttu-id="9954f-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9954f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

