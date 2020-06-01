---
title: ExtractAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc213f0e-a655-44e9-9ac9-bc1673bae1fe
description: L’élément ExtractAllowed spécifie si l’extraction d’entité est activée.
ms.openlocfilehash: f9fcae72d6241e51f549fbf650f5b2aebe019e46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461981"
---
# <a name="extractallowed"></a><span data-ttu-id="2d546-103">ExtractAllowed</span><span class="sxs-lookup"><span data-stu-id="2d546-103">ExtractAllowed</span></span>

<span data-ttu-id="2d546-104">L’élément **ExtractAllowed** spécifie si l’extraction d’entité est activée.</span><span class="sxs-lookup"><span data-stu-id="2d546-104">The **ExtractAllowed** element specifies whether entity extraction is enabled.</span></span> 
  
```XML
<ExtractAllowed>true | false</ExtractAllowed
```

 <span data-ttu-id="2d546-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2d546-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d546-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2d546-106">Attributes and elements</span></span>

<span data-ttu-id="2d546-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2d546-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d546-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2d546-108">Attributes</span></span>

<span data-ttu-id="2d546-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2d546-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d546-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2d546-110">Child elements</span></span>

<span data-ttu-id="2d546-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2d546-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2d546-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2d546-112">Parent elements</span></span>

|<span data-ttu-id="2d546-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2d546-113">**Element**</span></span>|<span data-ttu-id="2d546-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2d546-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d546-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="2d546-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="2d546-116">Spécifie les informations relatives à la licence de gestion des droits.</span><span class="sxs-lookup"><span data-stu-id="2d546-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2d546-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2d546-117">Text value</span></span>

<span data-ttu-id="2d546-118">Une valeur de texte de **true** pour l’élément **ExtractAllowed** indique que l’extraction d’entité est activée.</span><span class="sxs-lookup"><span data-stu-id="2d546-118">A text value of **true** for the **ExtractAllowed** element indicates that entity extraction is enabled.</span></span> <span data-ttu-id="2d546-119">La valeur **false** indique que l’extraction d’entité n’est pas activée.</span><span class="sxs-lookup"><span data-stu-id="2d546-119">A value of **false** indicates that entity extraction is not enabled.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2d546-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="2d546-120">Remarks</span></span>

<span data-ttu-id="2d546-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2d546-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2d546-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d546-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d546-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2d546-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d546-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2d546-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d546-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2d546-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2d546-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="2d546-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2d546-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="2d546-127">Validation File</span></span>  <br/> |<span data-ttu-id="2d546-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="2d546-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d546-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2d546-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2d546-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2d546-130">See also</span></span>



- [<span data-ttu-id="2d546-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2d546-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

