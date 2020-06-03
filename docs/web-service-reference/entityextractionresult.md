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
ms.openlocfilehash: f2f069717a5862adff3349090c35f95499d135f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456954"
---
# <a name="entityextractionresult"></a><span data-ttu-id="13997-103">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="13997-103">EntityExtractionResult</span></span>

<span data-ttu-id="13997-104">L’élément **EntityExtractionResult** spécifie la propriété **EntityExtractionResult** d’un élément.</span><span class="sxs-lookup"><span data-stu-id="13997-104">The **EntityExtractionResult** element specifies the **EntityExtractionResult** property of an item.</span></span> 
  
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

 <span data-ttu-id="13997-105">**EntityExtractionResultType**</span><span class="sxs-lookup"><span data-stu-id="13997-105">**EntityExtractionResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13997-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="13997-106">Attributes and elements</span></span>

<span data-ttu-id="13997-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="13997-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13997-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="13997-108">Attributes</span></span>

<span data-ttu-id="13997-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="13997-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="13997-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="13997-110">Child elements</span></span>

|<span data-ttu-id="13997-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="13997-111">**Element**</span></span>|<span data-ttu-id="13997-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="13997-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13997-113">Adresses (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="13997-113">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="13997-114">Spécifie un tableau d’éléments **AddressEntity** .</span><span class="sxs-lookup"><span data-stu-id="13997-114">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
|[<span data-ttu-id="13997-115">MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="13997-115">MeetingSuggestions</span></span>](meetingsuggestions.md) <br/> |<span data-ttu-id="13997-116">Spécifie un tableau d’éléments **MeetingSuggestion** .</span><span class="sxs-lookup"><span data-stu-id="13997-116">Specifies an array of **MeetingSuggestion** elements.</span></span>  <br/> |
|[<span data-ttu-id="13997-117">TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="13997-117">TaskSuggestions</span></span>](tasksuggestions.md) <br/> |<span data-ttu-id="13997-118">Spécifie un tableau d’éléments **TaskSuggestion** .</span><span class="sxs-lookup"><span data-stu-id="13997-118">Specifies an array of **TaskSuggestion** elements.</span></span>  <br/> |
|[<span data-ttu-id="13997-119">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="13997-119">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="13997-120">Spécifie un tableau d’entités d’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="13997-120">Specifies an array of email address entities.</span></span>  <br/> |
|[<span data-ttu-id="13997-121">Contacts (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="13997-121">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="13997-122">Spécifie un tableau de contacts.</span><span class="sxs-lookup"><span data-stu-id="13997-122">Specifies an array of contacts.</span></span>  <br/> |
|[<span data-ttu-id="13997-123">URL (ArrayOfUrlEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="13997-123">Urls (ArrayOfUrlEntitiesType)</span></span>](urls-arrayofurlentitiestype.md) <br/> |<span data-ttu-id="13997-124">Spécifie un tableau d’URL.</span><span class="sxs-lookup"><span data-stu-id="13997-124">Specifies an array of URLs.</span></span>  <br/> |
|[<span data-ttu-id="13997-125">PhoneNumbers (ArrayOfPhoneEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="13997-125">PhoneNumbers (ArrayOfPhoneEntitiesType)</span></span>](phonenumbers-arrayofphoneentitiestype.md) <br/> |<span data-ttu-id="13997-126">Spécifie un tableau de numéros de téléphone.</span><span class="sxs-lookup"><span data-stu-id="13997-126">Specifies an array of phone numbers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="13997-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="13997-127">Parent elements</span></span>

|<span data-ttu-id="13997-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="13997-128">**Element**</span></span>|<span data-ttu-id="13997-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="13997-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13997-130">Item</span><span class="sxs-lookup"><span data-stu-id="13997-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="13997-131">Représente un élément générique dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="13997-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="13997-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="13997-132">Remarks</span></span>

<span data-ttu-id="13997-133">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="13997-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="13997-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="13997-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13997-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="13997-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13997-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="13997-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="13997-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="13997-137">Schema Name</span></span>  <br/> |<span data-ttu-id="13997-138">Schéma type</span><span class="sxs-lookup"><span data-stu-id="13997-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="13997-139">Validation File</span><span class="sxs-lookup"><span data-stu-id="13997-139">Validation File</span></span>  <br/> |<span data-ttu-id="13997-140">types. xsd</span><span class="sxs-lookup"><span data-stu-id="13997-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="13997-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="13997-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="13997-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="13997-142">See also</span></span>



- [<span data-ttu-id="13997-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="13997-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

