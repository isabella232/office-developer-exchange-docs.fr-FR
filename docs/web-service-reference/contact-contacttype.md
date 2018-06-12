---
title: Contact (TypeContact)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: L’élément de Contact spécifie un contact dans le magasin de contacts unifié.
ms.openlocfilehash: f1593da78a46851c7db43abc567eb66c0c74e0f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755552"
---
# <a name="contact-contacttype"></a><span data-ttu-id="d8c39-103">Contact (TypeContact)</span><span class="sxs-lookup"><span data-stu-id="d8c39-103">Contact (ContactType)</span></span>

<span data-ttu-id="d8c39-104">L’élément de **Contact** spécifie un contact dans le magasin de contacts unifié.</span><span class="sxs-lookup"><span data-stu-id="d8c39-104">The **Contact** element specifies a contact in the Unified Contact Store.</span></span> 
  
```XML
<Contact>
    <PersonName></PersonName>
    <BusinessName></BusinessName>
    <PhoneNumbers></PhoneNumbers>
    <Urls></Urls>
    <EmailAddresses></EmailAddresses>
    <Addresses></Addesses>    <ContactString></ContactString
</Contact>
```

 <span data-ttu-id="d8c39-105">**TypeContact**</span><span class="sxs-lookup"><span data-stu-id="d8c39-105">**ContactType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8c39-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d8c39-106">Attributes and elements</span></span>

<span data-ttu-id="d8c39-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d8c39-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8c39-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d8c39-108">Attributes</span></span>

<span data-ttu-id="d8c39-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d8c39-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8c39-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d8c39-110">Child elements</span></span>

|<span data-ttu-id="d8c39-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d8c39-111">**Element**</span></span>|<span data-ttu-id="d8c39-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8c39-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8c39-113">PersonName</span><span class="sxs-lookup"><span data-stu-id="d8c39-113">PersonName</span></span>](personname.md) <br/> |<span data-ttu-id="d8c39-114">Spécifie le nom d’un participant.</span><span class="sxs-lookup"><span data-stu-id="d8c39-114">Specifies the name of an individual.</span></span>  <br/> |
|[<span data-ttu-id="d8c39-115">BusinessName</span><span class="sxs-lookup"><span data-stu-id="d8c39-115">BusinessName</span></span>](businessname.md) <br/> |<span data-ttu-id="d8c39-116">Spécifie le nom de l’entreprise.</span><span class="sxs-lookup"><span data-stu-id="d8c39-116">Specifies the name of a business.</span></span>  <br/> |
|[<span data-ttu-id="d8c39-117">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="d8c39-117">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="d8c39-118">Représente une collection de numéros de téléphone pour un contact.</span><span class="sxs-lookup"><span data-stu-id="d8c39-118">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="d8c39-119">URL</span><span class="sxs-lookup"><span data-stu-id="d8c39-119">Urls</span></span>](urls.md) <br/> |<span data-ttu-id="d8c39-120">Spécifie un tableau d’URL pour un personnage.</span><span class="sxs-lookup"><span data-stu-id="d8c39-120">Specifies an array of URLs for a persona.</span></span>  <br/> |
|[<span data-ttu-id="d8c39-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span><span class="sxs-lookup"><span data-stu-id="d8c39-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span></span>](emailaddresses-arrayofextractedemailaddresses.md) <br/> |<span data-ttu-id="d8c39-122">Spécifie un tableau des adresses de messagerie extraits.</span><span class="sxs-lookup"><span data-stu-id="d8c39-122">Specifies an array of extracted email addresses.</span></span>  <br/> |
|[<span data-ttu-id="d8c39-123">Adresses (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="d8c39-123">Addresses (ArrayOfAddressesType)</span></span>](addresses-arrayofaddressestype.md) <br/> |<span data-ttu-id="d8c39-124">Spécifie un tableau des éléments de **l’adresse** .</span><span class="sxs-lookup"><span data-stu-id="d8c39-124">Specifies an array of **Address** elements.</span></span>  <br/> |
|[<span data-ttu-id="d8c39-125">ContactString</span><span class="sxs-lookup"><span data-stu-id="d8c39-125">ContactString</span></span>](contactstring.md) <br/> |<span data-ttu-id="d8c39-126">Spécifie le nom complet d’un contact.</span><span class="sxs-lookup"><span data-stu-id="d8c39-126">Specifies the display name of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8c39-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d8c39-127">Parent elements</span></span>

|<span data-ttu-id="d8c39-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d8c39-128">**Element**</span></span>|<span data-ttu-id="d8c39-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8c39-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8c39-130">Contacts (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="d8c39-130">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="d8c39-131">Spécifie un tableau des contacts.</span><span class="sxs-lookup"><span data-stu-id="d8c39-131">Specifies an array of contacts.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d8c39-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="d8c39-132">Remarks</span></span>

<span data-ttu-id="d8c39-133">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d8c39-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d8c39-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8c39-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8c39-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d8c39-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8c39-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d8c39-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8c39-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d8c39-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d8c39-138">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d8c39-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="d8c39-139">Validation File</span><span class="sxs-lookup"><span data-stu-id="d8c39-139">Validation File</span></span>  <br/> |<span data-ttu-id="d8c39-140">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d8c39-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8c39-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d8c39-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d8c39-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d8c39-142">See also</span></span>



- [<span data-ttu-id="d8c39-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d8c39-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

