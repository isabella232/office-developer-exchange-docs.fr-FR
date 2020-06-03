---
title: IncludeUnsearchableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: L’élément IncludeUnsearchableItems spécifie s’il faut inclure les éléments qui ne peuvent pas être recherchés.
ms.openlocfilehash: 19fe450f5b1647be2df75138dbe67dd9e1c05c21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465701"
---
# <a name="includeunsearchableitems"></a><span data-ttu-id="2f795-103">IncludeUnsearchableItems</span><span class="sxs-lookup"><span data-stu-id="2f795-103">IncludeUnsearchableItems</span></span>

<span data-ttu-id="2f795-104">L’élément **IncludeUnsearchableItems** spécifie s’il faut inclure les éléments qui ne peuvent pas être recherchés.</span><span class="sxs-lookup"><span data-stu-id="2f795-104">The **IncludeUnsearchableItems** element specifies whether to include items that cannot be searched.</span></span> 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
```

 <span data-ttu-id="2f795-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2f795-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f795-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2f795-106">Attributes and elements</span></span>

<span data-ttu-id="2f795-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2f795-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f795-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2f795-108">Attributes</span></span>

<span data-ttu-id="2f795-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2f795-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f795-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2f795-110">Child elements</span></span>

<span data-ttu-id="2f795-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2f795-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2f795-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2f795-112">Parent elements</span></span>

|<span data-ttu-id="2f795-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2f795-113">**Element**</span></span>|<span data-ttu-id="2f795-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2f795-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f795-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="2f795-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="2f795-116">Spécifie une demande de recherche de statistiques de boîte aux lettres par mot clé.</span><span class="sxs-lookup"><span data-stu-id="2f795-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2f795-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2f795-117">Text value</span></span>

<span data-ttu-id="2f795-118">Une valeur de texte de **true** pour l’élément **IncludeUnsearchableItems** indique que les statistiques ne sont pas incluses pour les éléments qui ne peuvent pas faire l’objet d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="2f795-118">A text value of **true** for the **IncludeUnsearchableItems** element indicates that statistics are not included for items that are not searchable.</span></span> <span data-ttu-id="2f795-119">La valeur **false** indique que les statistiques sont incluses pour les éléments qui ne peuvent pas faire l’objet d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="2f795-119">A value of **false** indicates that statistics are included for items that are not searchable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2f795-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="2f795-120">Remarks</span></span>

<span data-ttu-id="2f795-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2f795-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2f795-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f795-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f795-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2f795-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f795-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2f795-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2f795-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2f795-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2f795-126">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="2f795-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="2f795-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2f795-127">Validation File</span></span>  <br/> |<span data-ttu-id="2f795-128">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2f795-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2f795-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2f795-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2f795-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2f795-130">See also</span></span>



- [<span data-ttu-id="2f795-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2f795-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

