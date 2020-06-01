---
title: Participants
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 837bb372-39eb-48ae-9c09-0d2552511f93
description: L’élément participants spécifie les destinataires d’une invitation à une réunion.
ms.openlocfilehash: 3a63bdf7e49309697ac503be5f4c95eb805b9635
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460329"
---
# <a name="attendees"></a><span data-ttu-id="e3359-103">Participants</span><span class="sxs-lookup"><span data-stu-id="e3359-103">Attendees</span></span>

<span data-ttu-id="e3359-104">L’élément **participants** spécifie les destinataires d’une invitation à une réunion.</span><span class="sxs-lookup"><span data-stu-id="e3359-104">The **Attendees** element specifies the recipients of an invitation to a meeting.</span></span> 
  
```XML
<Attendees>
    <EmailUser></EmailUser>
</Attendees>
```

 <span data-ttu-id="e3359-105">**ArrayOfEmailUsersType**</span><span class="sxs-lookup"><span data-stu-id="e3359-105">**ArrayOfEmailUsersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3359-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e3359-106">Attributes and elements</span></span>

<span data-ttu-id="e3359-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e3359-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3359-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e3359-108">Attributes</span></span>

<span data-ttu-id="e3359-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e3359-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3359-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e3359-110">Child elements</span></span>

|<span data-ttu-id="e3359-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e3359-111">**Element**</span></span>|<span data-ttu-id="e3359-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e3359-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3359-113">EmailUser</span><span class="sxs-lookup"><span data-stu-id="e3359-113">EmailUser</span></span>](emailuser.md) <br/> |<span data-ttu-id="e3359-114">Spécifie un destinataire de messagerie ou un contact Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e3359-114">Specifies an email recipient or Active Directory contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3359-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e3359-115">Parent elements</span></span>

|<span data-ttu-id="e3359-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e3359-116">**Element**</span></span>|<span data-ttu-id="e3359-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="e3359-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3359-118">MeetingSuggestion</span><span class="sxs-lookup"><span data-stu-id="e3359-118">MeetingSuggestion</span></span>](meetingsuggestion.md) <br/> |<span data-ttu-id="e3359-119">Spécifie une réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="e3359-119">Specifies a proposed meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e3359-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="e3359-120">Remarks</span></span>

<span data-ttu-id="e3359-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e3359-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e3359-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e3359-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3359-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e3359-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3359-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e3359-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3359-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e3359-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e3359-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="e3359-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e3359-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="e3359-127">Validation File</span></span>  <br/> |<span data-ttu-id="e3359-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="e3359-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3359-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e3359-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e3359-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e3359-130">See also</span></span>

- [<span data-ttu-id="e3359-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e3359-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

