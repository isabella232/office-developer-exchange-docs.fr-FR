---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: L’élément EntityExtractionResult spécifie la propriété EntityExtractionResult d’un élément.
ms.openlocfilehash: ef99629beb95f1e1123569fa99e3f495c1b56e95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756197"
---
# <a name="entityextractionresult"></a><span data-ttu-id="e20e6-103">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="e20e6-103">EntityExtractionResult</span></span>

<span data-ttu-id="e20e6-104">L’élément **EntityExtractionResult** spécifie la propriété **EntityExtractionResult** d’un élément.</span><span class="sxs-lookup"><span data-stu-id="e20e6-104">The **EntityExtractionResult** element specifies the **EntityExtractionResult** property of an item.</span></span> 
  
```XML
<EntityExtractionResult>
    <Addresses/>
    <MeetingSuggestions/>
    <TaskSuggestions/>
    <EmailAddresses/>
    <Contacts/>
    <Urls/>
    <PhoneNumbers/>
</EntityExtractionResult>
```

 <span data-ttu-id="e20e6-105">**EntityExtractionResultType**</span><span class="sxs-lookup"><span data-stu-id="e20e6-105">**EntityExtractionResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e20e6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e20e6-106">Attributes and elements</span></span>

<span data-ttu-id="e20e6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e20e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e20e6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e20e6-108">Attributes</span></span>

<span data-ttu-id="e20e6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e20e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e20e6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e20e6-110">Child elements</span></span>

|<span data-ttu-id="e20e6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e20e6-111">**Element**</span></span>|<span data-ttu-id="e20e6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e20e6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e20e6-113">Adresses (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="e20e6-113">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="e20e6-114">Spécifie un tableau d’éléments **AddressEntity** .</span><span class="sxs-lookup"><span data-stu-id="e20e6-114">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
|[<span data-ttu-id="e20e6-115">MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="e20e6-115">MeetingSuggestions</span></span>](meetingsuggestions.md) <br/> |<span data-ttu-id="e20e6-116">Spécifie un tableau d’éléments **MeetingSuggestion** .</span><span class="sxs-lookup"><span data-stu-id="e20e6-116">Specifies an array of **MeetingSuggestion** elements.</span></span>  <br/> |
|[<span data-ttu-id="e20e6-117">TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="e20e6-117">TaskSuggestions</span></span>](tasksuggestions.md) <br/> |<span data-ttu-id="e20e6-118">Spécifie un tableau d’éléments **TaskSuggestion** .</span><span class="sxs-lookup"><span data-stu-id="e20e6-118">Specifies an array of **TaskSuggestion** elements.</span></span>  <br/> |
|[<span data-ttu-id="e20e6-119">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="e20e6-119">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="e20e6-120">Spécifie un tableau des entités d’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="e20e6-120">Specifies an array of email address entities.</span></span>  <br/> |
|[<span data-ttu-id="e20e6-121">Contacts (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="e20e6-121">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="e20e6-122">Spécifie un tableau des contacts.</span><span class="sxs-lookup"><span data-stu-id="e20e6-122">Specifies an array of contacts.</span></span>  <br/> |
|[<span data-ttu-id="e20e6-123">URL (ArrayOfUrlEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="e20e6-123">Urls (ArrayOfUrlEntitiesType)</span></span>](urls-arrayofurlentitiestype.md) <br/> |<span data-ttu-id="e20e6-124">Spécifie un tableau d’URL.</span><span class="sxs-lookup"><span data-stu-id="e20e6-124">Specifies an array of URLs.</span></span>  <br/> |
|[<span data-ttu-id="e20e6-125">PhoneNumbers (ArrayOfPhoneEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="e20e6-125">PhoneNumbers (ArrayOfPhoneEntitiesType)</span></span>](phonenumbers-arrayofphoneentitiestype.md) <br/> |<span data-ttu-id="e20e6-126">Spécifie un tableau des numéros de téléphone.</span><span class="sxs-lookup"><span data-stu-id="e20e6-126">Specifies an array of phone numbers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e20e6-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e20e6-127">Parent elements</span></span>

|<span data-ttu-id="e20e6-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e20e6-128">**Element**</span></span>|<span data-ttu-id="e20e6-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="e20e6-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e20e6-130">Item</span><span class="sxs-lookup"><span data-stu-id="e20e6-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="e20e6-131">Représente un élément générique dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e20e6-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e20e6-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="e20e6-132">Remarks</span></span>

<span data-ttu-id="e20e6-133">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e20e6-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e20e6-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e20e6-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e20e6-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e20e6-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e20e6-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e20e6-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e20e6-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e20e6-137">Schema Name</span></span>  <br/> |<span data-ttu-id="e20e6-138">Schéma type</span><span class="sxs-lookup"><span data-stu-id="e20e6-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="e20e6-139">Validation File</span><span class="sxs-lookup"><span data-stu-id="e20e6-139">Validation File</span></span>  <br/> |<span data-ttu-id="e20e6-140">types.xsd</span><span class="sxs-lookup"><span data-stu-id="e20e6-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e20e6-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e20e6-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e20e6-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e20e6-142">See also</span></span>



- [<span data-ttu-id="e20e6-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e20e6-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

