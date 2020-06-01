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
ms.openlocfilehash: 7ba7be69868cb439177702f74ff4a2f12875b7ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468354"
---
# <a name="umenabled"></a><span data-ttu-id="f9d61-103">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="f9d61-103">UmEnabled</span></span>

<span data-ttu-id="f9d61-104">L’élément **UmEnabled** indique si la messagerie unifiée est activée pour un compte.</span><span class="sxs-lookup"><span data-stu-id="f9d61-104">The **UmEnabled** element indicates whether Unified Messaging is enabled for an account.</span></span> 
  
```XML
<UmEnabled>true | false</UmEnabled>
```

 <span data-ttu-id="f9d61-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f9d61-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9d61-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f9d61-106">Attributes and elements</span></span>

<span data-ttu-id="f9d61-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f9d61-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9d61-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f9d61-108">Attributes</span></span>

<span data-ttu-id="f9d61-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f9d61-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9d61-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f9d61-110">Child elements</span></span>

<span data-ttu-id="f9d61-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f9d61-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f9d61-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f9d61-112">Parent elements</span></span>

|<span data-ttu-id="f9d61-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f9d61-113">**Element**</span></span>|<span data-ttu-id="f9d61-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f9d61-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9d61-115">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9d61-115">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="f9d61-116">Contient des informations de configuration de service pour le service de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="f9d61-116">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f9d61-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f9d61-117">Text value</span></span>

<span data-ttu-id="f9d61-118">La valeur de texte de l’élément **UmEnabled** est **true** si la messagerie unifiée est activée pour le compte ; Sinon, la valeur est **false**.</span><span class="sxs-lookup"><span data-stu-id="f9d61-118">The text value of the **UmEnabled** element is **true** if Unified Messaging is enabled for the account; otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f9d61-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="f9d61-119">Remarks</span></span>

<span data-ttu-id="f9d61-120">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="f9d61-120">This element is required.</span></span>
  
<span data-ttu-id="f9d61-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9d61-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9d61-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f9d61-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9d61-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f9d61-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9d61-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f9d61-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f9d61-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f9d61-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9d61-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f9d61-126">Validation File</span></span>  <br/> |<span data-ttu-id="f9d61-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f9d61-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9d61-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f9d61-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9d61-129">False</span><span class="sxs-lookup"><span data-stu-id="f9d61-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9d61-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f9d61-130">See also</span></span>



- [<span data-ttu-id="f9d61-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f9d61-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

