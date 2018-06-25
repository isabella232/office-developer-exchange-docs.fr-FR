---
title: MailTipsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsEnabled
api_type:
- schema
ms.assetid: 737388b3-7b73-42af-94d3-3dbb0659718f
description: L’élément MailTipsEnabled indique si le service de conseils de messagerie est disponible.
ms.openlocfilehash: 4fe2cae1087ab667133ec685c3325b14c4f12088
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828330"
---
# <a name="mailtipsenabled"></a><span data-ttu-id="1ff95-103">MailTipsEnabled</span><span class="sxs-lookup"><span data-stu-id="1ff95-103">MailTipsEnabled</span></span>

<span data-ttu-id="1ff95-104">L’élément **MailTipsEnabled** indique si le service de conseils de messagerie est disponible.</span><span class="sxs-lookup"><span data-stu-id="1ff95-104">The **MailTipsEnabled** element indicates whether the mail tips service is available.</span></span> 
  
```xml
<MailTipsEnabled>true | false</MailTipsEnabled>
```

 <span data-ttu-id="1ff95-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1ff95-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ff95-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1ff95-106">Attributes and elements</span></span>

<span data-ttu-id="1ff95-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1ff95-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ff95-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1ff95-108">Attributes</span></span>

<span data-ttu-id="1ff95-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1ff95-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ff95-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1ff95-110">Child elements</span></span>

<span data-ttu-id="1ff95-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1ff95-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1ff95-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1ff95-112">Parent elements</span></span>

|<span data-ttu-id="1ff95-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1ff95-113">**Element**</span></span>|<span data-ttu-id="1ff95-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1ff95-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ff95-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="1ff95-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="1ff95-116">Contient des informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="1ff95-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1ff95-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1ff95-117">Text value</span></span>

<span data-ttu-id="1ff95-118">La valeur de texte de cet élément est **la valeur true** si le service de conseils de messagerie est disponible.</span><span class="sxs-lookup"><span data-stu-id="1ff95-118">The text value of this element is **true** if the mail tips service is available.</span></span> <span data-ttu-id="1ff95-119">La valeur est **false** si le service de conseils de messagerie n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="1ff95-119">The value is **false** if the mail tips service is not available.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1ff95-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="1ff95-120">Remarks</span></span>

<span data-ttu-id="1ff95-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ff95-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ff95-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1ff95-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ff95-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1ff95-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1ff95-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1ff95-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1ff95-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1ff95-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="1ff95-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1ff95-126">Validation File</span></span>  <br/> |<span data-ttu-id="1ff95-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1ff95-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1ff95-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1ff95-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ff95-129">False</span><span class="sxs-lookup"><span data-stu-id="1ff95-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ff95-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1ff95-130">See also</span></span>



- [<span data-ttu-id="1ff95-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1ff95-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

