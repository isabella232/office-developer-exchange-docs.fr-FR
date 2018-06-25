---
title: IncludeUnsearchableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: L’élément IncludeUnsearchableItems Spécifie s’il faut inclure des éléments qui ne peuvent pas être recherchés.
ms.openlocfilehash: 4c6b9b3752330bf914c9901d2e8f69e93546fec6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827907"
---
# <a name="includeunsearchableitems"></a><span data-ttu-id="ac835-103">IncludeUnsearchableItems</span><span class="sxs-lookup"><span data-stu-id="ac835-103">IncludeUnsearchableItems</span></span>

<span data-ttu-id="ac835-104">L’élément **IncludeUnsearchableItems** Spécifie s’il faut inclure des éléments qui ne peuvent pas être recherchés.</span><span class="sxs-lookup"><span data-stu-id="ac835-104">The **IncludeUnsearchableItems** element specifies whether to include items that cannot be searched.</span></span> 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
```

 <span data-ttu-id="ac835-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ac835-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac835-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ac835-106">Attributes and elements</span></span>

<span data-ttu-id="ac835-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ac835-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac835-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ac835-108">Attributes</span></span>

<span data-ttu-id="ac835-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ac835-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac835-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ac835-110">Child elements</span></span>

<span data-ttu-id="ac835-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ac835-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac835-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ac835-112">Parent elements</span></span>

|<span data-ttu-id="ac835-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ac835-113">**Element**</span></span>|<span data-ttu-id="ac835-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ac835-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac835-115">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="ac835-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="ac835-116">Spécifie une requête pour rechercher des statistiques de boîtes aux lettres par mot clé.</span><span class="sxs-lookup"><span data-stu-id="ac835-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac835-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ac835-117">Text value</span></span>

<span data-ttu-id="ac835-118">Une valeur de texte de **la valeur true** pour l’élément **IncludeUnsearchableItems** indique que les statistiques ne sont pas inclus pour les éléments qui ne sont pas utilisables dans une requête.</span><span class="sxs-lookup"><span data-stu-id="ac835-118">A text value of **true** for the **IncludeUnsearchableItems** element indicates that statistics are not included for items that are not searchable.</span></span> <span data-ttu-id="ac835-119">La valeur **false** indique que les statistiques sont inclus pour les éléments qui ne sont pas utilisables dans une requête.</span><span class="sxs-lookup"><span data-stu-id="ac835-119">A value of **false** indicates that statistics are included for items that are not searchable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ac835-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="ac835-120">Remarks</span></span>

<span data-ttu-id="ac835-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ac835-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ac835-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac835-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac835-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ac835-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac835-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ac835-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ac835-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ac835-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ac835-126">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="ac835-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="ac835-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ac835-127">Validation File</span></span>  <br/> |<span data-ttu-id="ac835-128">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ac835-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ac835-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ac835-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ac835-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ac835-130">See also</span></span>



- [<span data-ttu-id="ac835-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ac835-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

