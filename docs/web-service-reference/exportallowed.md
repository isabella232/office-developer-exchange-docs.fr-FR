---
title: ExportAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dcff5ccc-31dc-4941-9f71-d6519133aebb
description: L’élément ExportAllowed Spécifie si l’exportation est activée.
ms.openlocfilehash: 5c07941e0a79394bbdaa1a1f62b20adedfe7a9bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756262"
---
# <a name="exportallowed"></a><span data-ttu-id="2ee10-103">ExportAllowed</span><span class="sxs-lookup"><span data-stu-id="2ee10-103">ExportAllowed</span></span>

<span data-ttu-id="2ee10-104">L’élément **ExportAllowed** Spécifie si l’exportation est activée.</span><span class="sxs-lookup"><span data-stu-id="2ee10-104">The **ExportAllowed** element specifies whether exporting is enabled.</span></span> 
  
```XML
<ExportAllowed>true | false</ExportAllowed>
```

 <span data-ttu-id="2ee10-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2ee10-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ee10-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ee10-106">Attributes and elements</span></span>

<span data-ttu-id="2ee10-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ee10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ee10-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ee10-108">Attributes</span></span>

<span data-ttu-id="2ee10-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ee10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ee10-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ee10-110">Child elements</span></span>

<span data-ttu-id="2ee10-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ee10-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ee10-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ee10-112">Parent elements</span></span>

|<span data-ttu-id="2ee10-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ee10-113">**Element**</span></span>|<span data-ttu-id="2ee10-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ee10-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ee10-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="2ee10-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="2ee10-116">Spécifie des informations sur la licence de gestion des droits.</span><span class="sxs-lookup"><span data-stu-id="2ee10-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ee10-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2ee10-117">Text value</span></span>

<span data-ttu-id="2ee10-118">Une valeur de texte de **la valeur true** pour l’élément **ExportAllowed** indique que l’exportation est autorisée.</span><span class="sxs-lookup"><span data-stu-id="2ee10-118">A text value of **true** for the **ExportAllowed** element indicates that exporting is allowed.</span></span> <span data-ttu-id="2ee10-119">La valeur **false** indique que l’option exportation n’est pas autorisée.</span><span class="sxs-lookup"><span data-stu-id="2ee10-119">A value of **false** indicates that exporting is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2ee10-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="2ee10-120">Remarks</span></span>

<span data-ttu-id="2ee10-121">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="2ee10-121">This element is optional.</span></span>
  
<span data-ttu-id="2ee10-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2ee10-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2ee10-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ee10-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ee10-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ee10-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ee10-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ee10-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ee10-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ee10-126">Schema Name</span></span>  <br/> |<span data-ttu-id="2ee10-127">Schéma type</span><span class="sxs-lookup"><span data-stu-id="2ee10-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="2ee10-128">Validation File</span><span class="sxs-lookup"><span data-stu-id="2ee10-128">Validation File</span></span>  <br/> |<span data-ttu-id="2ee10-129">types.xsd</span><span class="sxs-lookup"><span data-stu-id="2ee10-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ee10-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ee10-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2ee10-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2ee10-131">See also</span></span>



- [<span data-ttu-id="2ee10-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2ee10-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

