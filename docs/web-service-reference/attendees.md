---
title: Participants
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 837bb372-39eb-48ae-9c09-0d2552511f93
description: L’élément de participants spécifie les destinataires d’une invitation à une réunion.
ms.openlocfilehash: 22d88bb092b416c553144496e133680b53f5d30e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755345"
---
# <a name="attendees"></a><span data-ttu-id="97e28-103">Participants</span><span class="sxs-lookup"><span data-stu-id="97e28-103">Attendees</span></span>

<span data-ttu-id="97e28-104">L’élément de **participants** spécifie les destinataires d’une invitation à une réunion.</span><span class="sxs-lookup"><span data-stu-id="97e28-104">The **Attendees** element specifies the recipients of an invitation to a meeting.</span></span> 
  
```XML
<Attendees>
    <EmailUser></EmailUser>
</Attendees>
```

 <span data-ttu-id="97e28-105">**ArrayOfEmailUsersType**</span><span class="sxs-lookup"><span data-stu-id="97e28-105">**ArrayOfEmailUsersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97e28-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="97e28-106">Attributes and elements</span></span>

<span data-ttu-id="97e28-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="97e28-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97e28-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="97e28-108">Attributes</span></span>

<span data-ttu-id="97e28-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="97e28-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97e28-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="97e28-110">Child elements</span></span>

|<span data-ttu-id="97e28-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="97e28-111">**Element**</span></span>|<span data-ttu-id="97e28-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="97e28-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97e28-113">EmailUser</span><span class="sxs-lookup"><span data-stu-id="97e28-113">EmailUser</span></span>](emailuser.md) <br/> |<span data-ttu-id="97e28-114">Spécifie un destinataire de courrier électronique ou un contact Active Directory.</span><span class="sxs-lookup"><span data-stu-id="97e28-114">Specifies an email recipient or Active Directory contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97e28-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="97e28-115">Parent elements</span></span>

|<span data-ttu-id="97e28-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="97e28-116">**Element**</span></span>|<span data-ttu-id="97e28-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="97e28-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97e28-118">MeetingSuggestion</span><span class="sxs-lookup"><span data-stu-id="97e28-118">MeetingSuggestion</span></span>](meetingsuggestion.md) <br/> |<span data-ttu-id="97e28-119">Spécifie une réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="97e28-119">Specifies a proposed meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97e28-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="97e28-120">Remarks</span></span>

<span data-ttu-id="97e28-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="97e28-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="97e28-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="97e28-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97e28-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="97e28-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97e28-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="97e28-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97e28-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="97e28-125">Schema Name</span></span>  <br/> |<span data-ttu-id="97e28-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="97e28-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="97e28-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="97e28-127">Validation File</span></span>  <br/> |<span data-ttu-id="97e28-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="97e28-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="97e28-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="97e28-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="97e28-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="97e28-130">See also</span></span>

- [<span data-ttu-id="97e28-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="97e28-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

