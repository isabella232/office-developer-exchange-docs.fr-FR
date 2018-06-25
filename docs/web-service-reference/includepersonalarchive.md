---
title: IncludePersonalArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b373bb1a-6b1d-4959-98a1-4c4ea62973bc
description: L’élément IncludePersonalArchive Spécifie s’il faut inclure l’archive personnelle dans la recherche.
ms.openlocfilehash: ba2dcaae3befd3595815c7281858e4fa8a738e0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827905"
---
# <a name="includepersonalarchive"></a><span data-ttu-id="83861-103">IncludePersonalArchive</span><span class="sxs-lookup"><span data-stu-id="83861-103">IncludePersonalArchive</span></span>

<span data-ttu-id="83861-104">L’élément **IncludePersonalArchive** Spécifie s’il faut inclure l’archive personnelle dans la recherche.</span><span class="sxs-lookup"><span data-stu-id="83861-104">The **IncludePersonalArchive** element specifies whether to include the personal archive in the search.</span></span> 
  
```XML
<IncludePersonalArchive>true | false</IncludePersonalArchive>
```

 <span data-ttu-id="83861-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="83861-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83861-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="83861-106">Attributes and elements</span></span>

<span data-ttu-id="83861-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="83861-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83861-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="83861-108">Attributes</span></span>

<span data-ttu-id="83861-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="83861-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83861-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="83861-110">Child elements</span></span>

<span data-ttu-id="83861-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="83861-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="83861-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="83861-112">Parent elements</span></span>

|<span data-ttu-id="83861-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="83861-113">**Element**</span></span>|<span data-ttu-id="83861-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="83861-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83861-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="83861-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="83861-116">Spécifie une requête pour rechercher des statistiques de boîtes aux lettres par mot clé.</span><span class="sxs-lookup"><span data-stu-id="83861-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="83861-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="83861-117">Text value</span></span>

<span data-ttu-id="83861-118">Une valeur de texte de **la valeur true** pour l’élément **IncludePersonalArchive** indique que l’archive personnelle est inclus dans la recherche.</span><span class="sxs-lookup"><span data-stu-id="83861-118">A text value of **true** for the **IncludePersonalArchive** element indicates that the personal archive is included in the search.</span></span> <span data-ttu-id="83861-119">La valeur **false** indique que l’archive personnelle n’est pas inclus dans la recherche.</span><span class="sxs-lookup"><span data-stu-id="83861-119">A value of **false** indicates that the personal archive is not included in the search.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="83861-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="83861-120">Remarks</span></span>

<span data-ttu-id="83861-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="83861-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83861-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="83861-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83861-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="83861-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="83861-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="83861-124">Schema Name</span></span>  <br/> |<span data-ttu-id="83861-125">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="83861-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="83861-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="83861-126">Validation File</span></span>  <br/> |<span data-ttu-id="83861-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="83861-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="83861-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="83861-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="83861-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="83861-129">See also</span></span>



- [<span data-ttu-id="83861-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="83861-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

