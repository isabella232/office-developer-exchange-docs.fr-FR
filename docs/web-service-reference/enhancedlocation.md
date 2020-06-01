---
title: EnhancedLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdfb74f-f33c-46ae-a7c7-451a5b0c6a59
description: L’élément EnhancedLocation spécifie les informations d’emplacement, telles que le nom, l’adresse et les notes facultatives relatives à un emplacement.
ms.openlocfilehash: 06ec800b763ef61af51da03ca8a340f6ac4d2a8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462956"
---
# <a name="enhancedlocation"></a><span data-ttu-id="cb8e7-103">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="cb8e7-103">EnhancedLocation</span></span>

<span data-ttu-id="cb8e7-104">L’élément **EnhancedLocation** spécifie les informations d’emplacement, telles que le nom, l’adresse et les notes facultatives relatives à un emplacement.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-104">The **EnhancedLocation** element specifies location information such as the name, address, and optional notes about a location.</span></span> 
  
```XML
<EnhancedLocation>
    <DisplayName/>
    <Annotation/>
    <PostalAddress/>
</EnhancedLocation>
```

 <span data-ttu-id="cb8e7-105">**EnhancedLocationType**</span><span class="sxs-lookup"><span data-stu-id="cb8e7-105">**EnhancedLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb8e7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cb8e7-106">Attributes and elements</span></span>

<span data-ttu-id="cb8e7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb8e7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cb8e7-108">Attributes</span></span>

<span data-ttu-id="cb8e7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb8e7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cb8e7-110">Child elements</span></span>

|<span data-ttu-id="cb8e7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cb8e7-111">**Element**</span></span>|<span data-ttu-id="cb8e7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="cb8e7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb8e7-113">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="cb8e7-113">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="cb8e7-114">Définit le nom d’affichage d’un dossier, d’un contact, d’une liste de distribution, d’un utilisateur délégué, d’un emplacement ou d’une règle.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-114">Defines the display name of a folder, contact, distribution list, delegate user, location, or rule.</span></span>  <br/> |
|[<span data-ttu-id="cb8e7-115">Commentaire</span><span class="sxs-lookup"><span data-stu-id="cb8e7-115">Annotation</span></span>](annotation.md) <br/> |<span data-ttu-id="cb8e7-116">Contient des notes facultatives ajoutées par un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-116">Contains optional notes added by a user.</span></span>  <br/> |
|[<span data-ttu-id="cb8e7-117">PostalAddress (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="cb8e7-117">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="cb8e7-118">Spécifie l’adresse postale d’un personnage.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-118">Specifies the postal address for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb8e7-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cb8e7-119">Parent elements</span></span>

|<span data-ttu-id="cb8e7-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cb8e7-120">**Element**</span></span>|<span data-ttu-id="cb8e7-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="cb8e7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb8e7-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="cb8e7-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="cb8e7-123">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="cb8e7-124">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="cb8e7-124">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="cb8e7-125">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-125">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cb8e7-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="cb8e7-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="cb8e7-127">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb8e7-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="cb8e7-128">Remarks</span></span>

<span data-ttu-id="cb8e7-129">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cb8e7-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb8e7-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb8e7-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cb8e7-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb8e7-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cb8e7-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cb8e7-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cb8e7-133">Schema Name</span></span>  <br/> |<span data-ttu-id="cb8e7-134">Schéma type</span><span class="sxs-lookup"><span data-stu-id="cb8e7-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="cb8e7-135">Validation File</span><span class="sxs-lookup"><span data-stu-id="cb8e7-135">Validation File</span></span>  <br/> |<span data-ttu-id="cb8e7-136">types. xsd</span><span class="sxs-lookup"><span data-stu-id="cb8e7-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="cb8e7-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cb8e7-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cb8e7-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cb8e7-138">See also</span></span>



- [<span data-ttu-id="cb8e7-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cb8e7-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

