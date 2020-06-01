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
ms.openlocfilehash: c090106a536f4f40908d364cc3c9c43f6fe42beb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456534"
---
# <a name="emailuser"></a><span data-ttu-id="9a3e7-103">EmailUser</span><span class="sxs-lookup"><span data-stu-id="9a3e7-103">EmailUser</span></span>

<span data-ttu-id="9a3e7-104">L’élément **EmailUser** spécifie un destinataire de courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-104">The **EmailUser** element specifies an email recipient.</span></span> 
  
```XML
<EmailUser>
    <Name/>
    <UserId/>
</EmailUser>
```

 <span data-ttu-id="9a3e7-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="9a3e7-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a3e7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9a3e7-106">Attributes and elements</span></span>

<span data-ttu-id="9a3e7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a3e7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9a3e7-108">Attributes</span></span>

<span data-ttu-id="9a3e7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a3e7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9a3e7-110">Child elements</span></span>

|<span data-ttu-id="9a3e7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a3e7-111">**Element**</span></span>|<span data-ttu-id="9a3e7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a3e7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a3e7-113">Nom (chaîne)</span><span class="sxs-lookup"><span data-stu-id="9a3e7-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="9a3e7-114">Spécifie un nom de l’affinement de recherche ou une clé ou le nom d’un utilisateur de messagerie.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="9a3e7-115">UserId (String)</span><span class="sxs-lookup"><span data-stu-id="9a3e7-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="9a3e7-116">Spécifie l’identificateur d’utilisateur d’un utilisateur de messagerie.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a3e7-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9a3e7-117">Parent elements</span></span>

|<span data-ttu-id="9a3e7-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a3e7-118">**Element**</span></span>|<span data-ttu-id="9a3e7-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a3e7-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a3e7-120">Participants</span><span class="sxs-lookup"><span data-stu-id="9a3e7-120">Attendees</span></span>](attendees.md) <br/> |<span data-ttu-id="9a3e7-121">Spécifie les destinataires d’une invitation à une réunion.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-121">Specifies the recipients of an invitation to a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9a3e7-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="9a3e7-122">Remarks</span></span>

<span data-ttu-id="9a3e7-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9a3e7-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9a3e7-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a3e7-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9a3e7-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a3e7-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9a3e7-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9a3e7-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9a3e7-127">Schema Name</span></span>  <br/> |<span data-ttu-id="9a3e7-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="9a3e7-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="9a3e7-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="9a3e7-129">Validation File</span></span>  <br/> |<span data-ttu-id="9a3e7-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="9a3e7-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9a3e7-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9a3e7-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9a3e7-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9a3e7-132">See also</span></span>



- [<span data-ttu-id="9a3e7-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9a3e7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

