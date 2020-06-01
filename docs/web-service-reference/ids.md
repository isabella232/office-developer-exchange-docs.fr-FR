---
title: Codes
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
description: L’élément IDS contient un tableau d’identificateurs de définition de fuseau horaire.
ms.openlocfilehash: 1c5a6974c8d3abc318ff122f3db09d8c3472dc65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457619"
---
# <a name="ids"></a><span data-ttu-id="8636a-103">Codes</span><span class="sxs-lookup"><span data-stu-id="8636a-103">Ids</span></span>

<span data-ttu-id="8636a-104">L’élément **IDS** contient un tableau d’identificateurs de définition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="8636a-104">The **Ids** element contains an array of time zone definition identifiers.</span></span> 
  
```XML
<Ids>
   <Id/>
</Ids>
```

 <span data-ttu-id="8636a-105">**NonEmptyArrayOfTimeZoneIdType**</span><span class="sxs-lookup"><span data-stu-id="8636a-105">**NonEmptyArrayOfTimeZoneIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8636a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8636a-106">Attributes and elements</span></span>

<span data-ttu-id="8636a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8636a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8636a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8636a-108">Attributes</span></span>

<span data-ttu-id="8636a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8636a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8636a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8636a-110">Child elements</span></span>

|<span data-ttu-id="8636a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8636a-111">**Element**</span></span>|<span data-ttu-id="8636a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8636a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8636a-113">ID (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="8636a-113">Id (TimeZone)</span></span>](id-timezone.md) <br/> |<span data-ttu-id="8636a-114">Élément qui identifie une définition de fuseau horaire unique.</span><span class="sxs-lookup"><span data-stu-id="8636a-114">The element that identifies a single time zone definition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8636a-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8636a-115">Parent elements</span></span>

|<span data-ttu-id="8636a-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8636a-116">**Element**</span></span>|<span data-ttu-id="8636a-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="8636a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8636a-118">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="8636a-118">GetServerTimeZones</span></span>](getservertimezones.md) <br/> |<span data-ttu-id="8636a-119">Définit une demande de récupération des définitions de fuseau horaire à partir du serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="8636a-119">Defines a request to retrieve time zone definitions from the Exchange server.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="8636a-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8636a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8636a-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8636a-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8636a-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8636a-122">Schema Name</span></span>  <br/> |<span data-ttu-id="8636a-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8636a-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8636a-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8636a-124">Validation File</span></span>  <br/> |<span data-ttu-id="8636a-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8636a-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8636a-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8636a-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="8636a-127">False</span><span class="sxs-lookup"><span data-stu-id="8636a-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8636a-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8636a-128">See also</span></span>



- [<span data-ttu-id="8636a-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8636a-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

