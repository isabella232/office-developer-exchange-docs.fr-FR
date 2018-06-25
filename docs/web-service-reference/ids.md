---
title: ID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Ids
api_type:
- schema
ms.assetid: c54cdeaf-6761-4d1a-a329-fb279f0e2a64
description: L’élément ID contient un tableau d’identificateurs de définition de fuseau horaire.
ms.openlocfilehash: e4f8afb1292b3cb9f3990d4613b7461050976a59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827856"
---
# <a name="ids"></a><span data-ttu-id="c9755-103">ID</span><span class="sxs-lookup"><span data-stu-id="c9755-103">Ids</span></span>

<span data-ttu-id="c9755-104">L’élément **ID** contient un tableau d’identificateurs de définition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="c9755-104">The **Ids** element contains an array of time zone definition identifiers.</span></span> 
  
```XML
<Ids>
   <Id/>
</Ids>
```

 <span data-ttu-id="c9755-105">**NonEmptyArrayOfTimeZoneIdType**</span><span class="sxs-lookup"><span data-stu-id="c9755-105">**NonEmptyArrayOfTimeZoneIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9755-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c9755-106">Attributes and elements</span></span>

<span data-ttu-id="c9755-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c9755-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9755-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c9755-108">Attributes</span></span>

<span data-ttu-id="c9755-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c9755-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9755-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c9755-110">Child elements</span></span>

|<span data-ttu-id="c9755-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c9755-111">**Element**</span></span>|<span data-ttu-id="c9755-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c9755-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9755-113">ID (fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="c9755-113">Id (TimeZone)</span></span>](id-timezone.md) <br/> |<span data-ttu-id="c9755-114">L’élément qui identifie une définition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="c9755-114">The element that identifies a single time zone definition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9755-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c9755-115">Parent elements</span></span>

|<span data-ttu-id="c9755-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c9755-116">**Element**</span></span>|<span data-ttu-id="c9755-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c9755-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9755-118">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="c9755-118">GetServerTimeZones</span></span>](getservertimezones.md) <br/> |<span data-ttu-id="c9755-119">Définit une requête pour récupérer les définitions de fuseau horaire à partir du serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9755-119">Defines a request to retrieve time zone definitions from the Exchange server.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="c9755-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c9755-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9755-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c9755-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c9755-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c9755-122">Schema Name</span></span>  <br/> |<span data-ttu-id="c9755-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c9755-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c9755-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c9755-124">Validation File</span></span>  <br/> |<span data-ttu-id="c9755-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c9755-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9755-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c9755-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9755-127">False</span><span class="sxs-lookup"><span data-stu-id="c9755-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9755-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c9755-128">See also</span></span>



- [<span data-ttu-id="c9755-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c9755-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

