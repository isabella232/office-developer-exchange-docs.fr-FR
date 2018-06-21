---
title: UmEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UmEnabled
api_type:
- schema
ms.assetid: 87382d9b-0c02-49ec-85dc-3f5918df3195
description: L’élément UmEnabled indique si la messagerie unifiée est activée pour un compte.
ms.openlocfilehash: 8324e02136adc6704bc0badb77131e9671ee569f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19838793"
---
# <a name="umenabled"></a><span data-ttu-id="dd858-103">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="dd858-103">UmEnabled</span></span>

<span data-ttu-id="dd858-104">L’élément **UmEnabled** indique si la messagerie unifiée est activée pour un compte.</span><span class="sxs-lookup"><span data-stu-id="dd858-104">The **UmEnabled** element indicates whether Unified Messaging is enabled for an account.</span></span> 
  
```XML
<UmEnabled>true | false</UmEnabled>
```

 <span data-ttu-id="dd858-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="dd858-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd858-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dd858-106">Attributes and elements</span></span>

<span data-ttu-id="dd858-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dd858-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd858-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dd858-108">Attributes</span></span>

<span data-ttu-id="dd858-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dd858-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd858-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dd858-110">Child elements</span></span>

<span data-ttu-id="dd858-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dd858-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd858-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dd858-112">Parent elements</span></span>

|<span data-ttu-id="dd858-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dd858-113">**Element**</span></span>|<span data-ttu-id="dd858-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="dd858-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd858-115">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="dd858-115">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="dd858-116">Contient des informations de configuration de service pour le service de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="dd858-116">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd858-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="dd858-117">Text value</span></span>

<span data-ttu-id="dd858-118">La valeur de texte de l’élément **UmEnabled** a la **valeur true** si la messagerie unifiée est activée pour le compte. dans le cas contraire, la valeur est **false**.</span><span class="sxs-lookup"><span data-stu-id="dd858-118">The text value of the **UmEnabled** element is **true** if Unified Messaging is enabled for the account; otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd858-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="dd858-119">Remarks</span></span>

<span data-ttu-id="dd858-120">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="dd858-120">This element is required.</span></span>
  
<span data-ttu-id="dd858-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd858-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd858-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dd858-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd858-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dd858-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd858-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dd858-124">Schema Name</span></span>  <br/> |<span data-ttu-id="dd858-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="dd858-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd858-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dd858-126">Validation File</span></span>  <br/> |<span data-ttu-id="dd858-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dd858-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd858-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dd858-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd858-129">False</span><span class="sxs-lookup"><span data-stu-id="dd858-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd858-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dd858-130">See also</span></span>



- [<span data-ttu-id="dd858-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dd858-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

