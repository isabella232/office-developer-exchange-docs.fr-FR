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
ms.openlocfilehash: b76b08f93e60c8492906f3cc94e60f5725c8a9dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526220"
---
# <a name="emailaddressentity"></a><span data-ttu-id="f19c3-103">EmailAddressEntity</span><span class="sxs-lookup"><span data-stu-id="f19c3-103">EmailAddressEntity</span></span>

<span data-ttu-id="f19c3-104">L’élément **EmailAddressEntity** spécifie une entité d’adresse de messagerie unique.</span><span class="sxs-lookup"><span data-stu-id="f19c3-104">The **EmailAddressEntity** element specifies a single email address entity.</span></span> 
  
```XML
<EmailAddressEntity>
    <EmailAddress></EmailAddress>
</EmailAddressEntity>
```

 <span data-ttu-id="f19c3-105">**EmailAddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="f19c3-105">**EmailAddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f19c3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f19c3-106">Attributes and elements</span></span>

<span data-ttu-id="f19c3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f19c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f19c3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f19c3-108">Attributes</span></span>

<span data-ttu-id="f19c3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f19c3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f19c3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f19c3-110">Child elements</span></span>

|<span data-ttu-id="f19c3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f19c3-111">**Element**</span></span>|<span data-ttu-id="f19c3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f19c3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f19c3-113">EmailAddress (chaîne)</span><span class="sxs-lookup"><span data-stu-id="f19c3-113">EmailAddress (string)</span></span>](emailaddress-string.md) <br/> |<span data-ttu-id="f19c3-114">Spécifie une adresse de messagerie unique.</span><span class="sxs-lookup"><span data-stu-id="f19c3-114">Specifies a single email address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f19c3-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f19c3-115">Parent elements</span></span>

|<span data-ttu-id="f19c3-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f19c3-116">**Element**</span></span>|<span data-ttu-id="f19c3-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="f19c3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f19c3-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="f19c3-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="f19c3-119">Spécifie un tableau d’entités d’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="f19c3-119">Specifies an array of email address entities.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f19c3-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="f19c3-120">Remarks</span></span>

<span data-ttu-id="f19c3-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f19c3-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f19c3-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f19c3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f19c3-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f19c3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f19c3-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f19c3-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f19c3-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f19c3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f19c3-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="f19c3-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f19c3-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="f19c3-127">Validation File</span></span>  <br/> |<span data-ttu-id="f19c3-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="f19c3-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f19c3-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f19c3-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f19c3-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f19c3-130">See also</span></span>



- [<span data-ttu-id="f19c3-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f19c3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

