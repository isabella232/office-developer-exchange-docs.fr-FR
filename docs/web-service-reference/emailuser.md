---
title: EmailUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc8133ff-c34e-4921-bb56-06e79aee0a8a
description: L’élément EmailUser spécifie un destinataire de courrier électronique.
ms.openlocfilehash: e724b3996d37a42527ec1183cef9bb6b312b8c93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756150"
---
# <a name="emailuser"></a><span data-ttu-id="fd274-103">EmailUser</span><span class="sxs-lookup"><span data-stu-id="fd274-103">EmailUser</span></span>

<span data-ttu-id="fd274-104">L’élément **EmailUser** spécifie un destinataire de courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="fd274-104">The **EmailUser** element specifies an email recipient.</span></span> 
  
```XML
<EmailUser>
    <Name/>
    <UserId/>
</EmailUser>
```

 <span data-ttu-id="fd274-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="fd274-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd274-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fd274-106">Attributes and elements</span></span>

<span data-ttu-id="fd274-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fd274-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd274-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fd274-108">Attributes</span></span>

<span data-ttu-id="fd274-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fd274-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd274-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fd274-110">Child elements</span></span>

|<span data-ttu-id="fd274-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fd274-111">**Element**</span></span>|<span data-ttu-id="fd274-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd274-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd274-113">Name (chaîne)</span><span class="sxs-lookup"><span data-stu-id="fd274-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="fd274-114">Spécifie un nom d’affinement de recherche ou la clé ou le nom d’un utilisateur de messagerie.</span><span class="sxs-lookup"><span data-stu-id="fd274-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="fd274-115">Nom d’utilisateur (chaîne)</span><span class="sxs-lookup"><span data-stu-id="fd274-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="fd274-116">Spécifie l’identificateur d’utilisateur d’un utilisateur de messagerie.</span><span class="sxs-lookup"><span data-stu-id="fd274-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd274-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fd274-117">Parent elements</span></span>

|<span data-ttu-id="fd274-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fd274-118">**Element**</span></span>|<span data-ttu-id="fd274-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd274-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd274-120">Participants</span><span class="sxs-lookup"><span data-stu-id="fd274-120">Attendees</span></span>](attendees.md) <br/> |<span data-ttu-id="fd274-121">Spécifie les destinataires d’une invitation à une réunion.</span><span class="sxs-lookup"><span data-stu-id="fd274-121">Specifies the recipients of an invitation to a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fd274-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="fd274-122">Remarks</span></span>

<span data-ttu-id="fd274-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fd274-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fd274-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd274-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd274-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fd274-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd274-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fd274-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd274-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fd274-127">Schema Name</span></span>  <br/> |<span data-ttu-id="fd274-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="fd274-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="fd274-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="fd274-129">Validation File</span></span>  <br/> |<span data-ttu-id="fd274-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="fd274-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd274-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fd274-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fd274-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fd274-132">See also</span></span>



- [<span data-ttu-id="fd274-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fd274-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

