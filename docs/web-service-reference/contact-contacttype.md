---
title: Contact (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: L’élément contact spécifie un contact dans le magasin de contacts unifié.
ms.openlocfilehash: e8ebc28456f8bfc26f5d790ac9ff278930041ea0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461519"
---
# <a name="contact-contacttype"></a><span data-ttu-id="d2234-103">Contact (ContactType)</span><span class="sxs-lookup"><span data-stu-id="d2234-103">Contact (ContactType)</span></span>

<span data-ttu-id="d2234-104">L’élément **contact** spécifie un contact dans le magasin de contacts unifié.</span><span class="sxs-lookup"><span data-stu-id="d2234-104">The **Contact** element specifies a contact in the Unified Contact Store.</span></span> 
  
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

 <span data-ttu-id="d2234-105">**ContactType**</span><span class="sxs-lookup"><span data-stu-id="d2234-105">**ContactType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2234-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d2234-106">Attributes and elements</span></span>

<span data-ttu-id="d2234-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d2234-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2234-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d2234-108">Attributes</span></span>

<span data-ttu-id="d2234-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d2234-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2234-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d2234-110">Child elements</span></span>

|<span data-ttu-id="d2234-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2234-111">**Element**</span></span>|<span data-ttu-id="d2234-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2234-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2234-113">PersonName</span><span class="sxs-lookup"><span data-stu-id="d2234-113">PersonName</span></span>](personname.md) <br/> |<span data-ttu-id="d2234-114">Spécifie le nom d’un individu.</span><span class="sxs-lookup"><span data-stu-id="d2234-114">Specifies the name of an individual.</span></span>  <br/> |
|[<span data-ttu-id="d2234-115">BusinessName</span><span class="sxs-lookup"><span data-stu-id="d2234-115">BusinessName</span></span>](businessname.md) <br/> |<span data-ttu-id="d2234-116">Spécifie le nom d’une entreprise.</span><span class="sxs-lookup"><span data-stu-id="d2234-116">Specifies the name of a business.</span></span>  <br/> |
|[<span data-ttu-id="d2234-117">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="d2234-117">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="d2234-118">Représente une collection de numéros de téléphone pour un contact.</span><span class="sxs-lookup"><span data-stu-id="d2234-118">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
|[<span data-ttu-id="d2234-119">URL</span><span class="sxs-lookup"><span data-stu-id="d2234-119">Urls</span></span>](urls.md) <br/> |<span data-ttu-id="d2234-120">Spécifie un tableau d’URL pour un personnage.</span><span class="sxs-lookup"><span data-stu-id="d2234-120">Specifies an array of URLs for a persona.</span></span>  <br/> |
|[<span data-ttu-id="d2234-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span><span class="sxs-lookup"><span data-stu-id="d2234-121">EmailAddresses (ArrayOfExtractedEmailAddresses)</span></span>](emailaddresses-arrayofextractedemailaddresses.md) <br/> |<span data-ttu-id="d2234-122">Spécifie un tableau d’adresses de messagerie extraites.</span><span class="sxs-lookup"><span data-stu-id="d2234-122">Specifies an array of extracted email addresses.</span></span>  <br/> |
|[<span data-ttu-id="d2234-123">Adresses (ArrayOfAddressesType)</span><span class="sxs-lookup"><span data-stu-id="d2234-123">Addresses (ArrayOfAddressesType)</span></span>](addresses-arrayofaddressestype.md) <br/> |<span data-ttu-id="d2234-124">Spécifie un tableau d’éléments **Address** .</span><span class="sxs-lookup"><span data-stu-id="d2234-124">Specifies an array of **Address** elements.</span></span>  <br/> |
|[<span data-ttu-id="d2234-125">ContactString</span><span class="sxs-lookup"><span data-stu-id="d2234-125">ContactString</span></span>](contactstring.md) <br/> |<span data-ttu-id="d2234-126">Spécifie le nom d’affichage d’un contact.</span><span class="sxs-lookup"><span data-stu-id="d2234-126">Specifies the display name of a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2234-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d2234-127">Parent elements</span></span>

|<span data-ttu-id="d2234-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2234-128">**Element**</span></span>|<span data-ttu-id="d2234-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2234-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2234-130">Contacts (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="d2234-130">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="d2234-131">Spécifie un tableau de contacts.</span><span class="sxs-lookup"><span data-stu-id="d2234-131">Specifies an array of contacts.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2234-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="d2234-132">Remarks</span></span>

<span data-ttu-id="d2234-133">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d2234-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d2234-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2234-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2234-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d2234-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2234-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d2234-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2234-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d2234-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d2234-138">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d2234-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="d2234-139">Validation File</span><span class="sxs-lookup"><span data-stu-id="d2234-139">Validation File</span></span>  <br/> |<span data-ttu-id="d2234-140">types. xsd</span><span class="sxs-lookup"><span data-stu-id="d2234-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2234-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d2234-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d2234-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d2234-142">See also</span></span>



- [<span data-ttu-id="d2234-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d2234-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

