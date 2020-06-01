---
title: EmailAddresses (ArrayOfEmailAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95084659-aa5a-4bac-8977-00db3b87883e
description: L’élément EmailAddresses spécifie un tableau de toutes les adresses de messagerie du personnage associé.
ms.openlocfilehash: e6132e9ef4ed13ea2546783f65d184fafeed5530
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463418"
---
# <a name="emailaddresses-arrayofemailaddressestype"></a><span data-ttu-id="d248b-103">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="d248b-103">EmailAddresses (ArrayOfEmailAddressesType)</span></span>

<span data-ttu-id="d248b-104">L’élément **EmailAddresses** spécifie un tableau de toutes les adresses de messagerie du personnage associé.</span><span class="sxs-lookup"><span data-stu-id="d248b-104">The **EmailAddresses** element specifies an array of all email addresses of the associated persona.</span></span> 
  
```XML
<EmailAddresses>
    <Address></Address>
</EmailAddresses>
```

 <span data-ttu-id="d248b-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="d248b-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d248b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d248b-106">Attributes and elements</span></span>

<span data-ttu-id="d248b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d248b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d248b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d248b-108">Attributes</span></span>

<span data-ttu-id="d248b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d248b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d248b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d248b-110">Child elements</span></span>

|<span data-ttu-id="d248b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d248b-111">**Element**</span></span>|<span data-ttu-id="d248b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d248b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d248b-113">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d248b-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="d248b-114">Représente une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="d248b-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d248b-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d248b-115">Parent elements</span></span>

|<span data-ttu-id="d248b-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d248b-116">**Element**</span></span>|<span data-ttu-id="d248b-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d248b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d248b-118">Persona</span><span class="sxs-lookup"><span data-stu-id="d248b-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="d248b-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="d248b-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d248b-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="d248b-120">Remarks</span></span>

<span data-ttu-id="d248b-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d248b-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d248b-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d248b-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d248b-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d248b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d248b-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d248b-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d248b-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d248b-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d248b-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d248b-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d248b-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="d248b-127">Validation File</span></span>  <br/> |<span data-ttu-id="d248b-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="d248b-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d248b-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d248b-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d248b-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d248b-130">See also</span></span>



- [<span data-ttu-id="d248b-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d248b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

