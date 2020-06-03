---
title: IncludePersonalArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b373bb1a-6b1d-4959-98a1-4c4ea62973bc
description: L’élément IncludePersonalArchive spécifie s’il faut inclure l’archive personnelle dans la recherche.
ms.openlocfilehash: a25dd45bc0717af8f949d14b88793af3821ca69f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458249"
---
# <a name="includepersonalarchive"></a><span data-ttu-id="ac357-103">IncludePersonalArchive</span><span class="sxs-lookup"><span data-stu-id="ac357-103">IncludePersonalArchive</span></span>

<span data-ttu-id="ac357-104">L’élément **IncludePersonalArchive** spécifie s’il faut inclure l’archive personnelle dans la recherche.</span><span class="sxs-lookup"><span data-stu-id="ac357-104">The **IncludePersonalArchive** element specifies whether to include the personal archive in the search.</span></span> 
  
```XML
<IncludePersonalArchive>true | false</IncludePersonalArchive>
```

 <span data-ttu-id="ac357-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ac357-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac357-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ac357-106">Attributes and elements</span></span>

<span data-ttu-id="ac357-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ac357-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac357-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ac357-108">Attributes</span></span>

<span data-ttu-id="ac357-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ac357-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac357-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ac357-110">Child elements</span></span>

<span data-ttu-id="ac357-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ac357-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac357-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ac357-112">Parent elements</span></span>

|<span data-ttu-id="ac357-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ac357-113">**Element**</span></span>|<span data-ttu-id="ac357-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ac357-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac357-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="ac357-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="ac357-116">Spécifie une demande de recherche de statistiques de boîte aux lettres par mot clé.</span><span class="sxs-lookup"><span data-stu-id="ac357-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac357-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ac357-117">Text value</span></span>

<span data-ttu-id="ac357-118">Une valeur de texte de **true** pour l’élément **IncludePersonalArchive** indique que l’archive personnelle est incluse dans la recherche.</span><span class="sxs-lookup"><span data-stu-id="ac357-118">A text value of **true** for the **IncludePersonalArchive** element indicates that the personal archive is included in the search.</span></span> <span data-ttu-id="ac357-119">La valeur **false** indique que l’archive personnelle n’est pas incluse dans la recherche.</span><span class="sxs-lookup"><span data-stu-id="ac357-119">A value of **false** indicates that the personal archive is not included in the search.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ac357-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="ac357-120">Remarks</span></span>

<span data-ttu-id="ac357-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac357-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac357-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ac357-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac357-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ac357-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ac357-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ac357-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ac357-125">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="ac357-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="ac357-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ac357-126">Validation File</span></span>  <br/> |<span data-ttu-id="ac357-127">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ac357-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ac357-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ac357-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ac357-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ac357-129">See also</span></span>



- [<span data-ttu-id="ac357-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ac357-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

