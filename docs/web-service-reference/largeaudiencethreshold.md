---
title: LargeAudienceThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LargeAudienceThreshold
api_type:
- schema
ms.assetid: dacd9db7-b8f0-445d-a3d1-3356b8c2bcd1
description: L’élément LargeAudienceThreshold représente le seuil d’audience important pour un client.
ms.openlocfilehash: 6d85f9eaf8b7723713877d376876461befa92324
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466387"
---
# <a name="largeaudiencethreshold"></a><span data-ttu-id="59311-103">LargeAudienceThreshold</span><span class="sxs-lookup"><span data-stu-id="59311-103">LargeAudienceThreshold</span></span>

<span data-ttu-id="59311-104">L’élément **LargeAudienceThreshold** représente le seuil d’audience important pour un client.</span><span class="sxs-lookup"><span data-stu-id="59311-104">The **LargeAudienceThreshold** element represents the large audience threshold for a client.</span></span> 
  
```XML
<LargeAudienceThreshold/>
```

 <span data-ttu-id="59311-105">**int**</span><span class="sxs-lookup"><span data-stu-id="59311-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59311-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59311-106">Attributes and elements</span></span>

<span data-ttu-id="59311-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59311-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59311-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="59311-108">Attributes</span></span>

<span data-ttu-id="59311-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="59311-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59311-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59311-110">Child elements</span></span>

<span data-ttu-id="59311-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59311-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59311-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59311-112">Parent elements</span></span>

|<span data-ttu-id="59311-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59311-113">**Element**</span></span>|<span data-ttu-id="59311-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="59311-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59311-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="59311-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="59311-116">Contient les informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="59311-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="59311-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="59311-117">Text value</span></span>

<span data-ttu-id="59311-118">La valeur de texte est un entier qui représente le seuil d’audience qui indique que le message est destiné à plusieurs personnes.</span><span class="sxs-lookup"><span data-stu-id="59311-118">The text value is an integer that represents the audience threshold that indicates that the message is going to more than one person.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="59311-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="59311-119">Remarks</span></span>

<span data-ttu-id="59311-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="59311-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59311-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="59311-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59311-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="59311-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59311-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="59311-123">Schema Name</span></span>  <br/> |<span data-ttu-id="59311-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="59311-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="59311-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="59311-125">Validation File</span></span>  <br/> |<span data-ttu-id="59311-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="59311-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59311-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="59311-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="59311-128">False</span><span class="sxs-lookup"><span data-stu-id="59311-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59311-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59311-129">See also</span></span>



- [<span data-ttu-id="59311-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="59311-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

