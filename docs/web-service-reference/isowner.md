---
title: IsOwner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea0f0afc-32fe-46cb-8530-62a6ce9490f6
description: L’élément IsOwner indique si l’utilisateur de messagerie spécifiée est le propriétaire.
ms.openlocfilehash: aac3c2a599093282542025468d73c55ec4569e29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828080"
---
# <a name="isowner"></a><span data-ttu-id="d631c-103">IsOwner</span><span class="sxs-lookup"><span data-stu-id="d631c-103">IsOwner</span></span>

<span data-ttu-id="d631c-104">L’élément **IsOwner** indique si l’utilisateur de messagerie spécifiée est le propriétaire.</span><span class="sxs-lookup"><span data-stu-id="d631c-104">The **IsOwner** element specifies whether the specified email user is the owner.</span></span> 
  
```XML
<IsOwner>true | false</IsOwner>
```

 <span data-ttu-id="d631c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d631c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d631c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d631c-106">Attributes and elements</span></span>

<span data-ttu-id="d631c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d631c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d631c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d631c-108">Attributes</span></span>

<span data-ttu-id="d631c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d631c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d631c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d631c-110">Child elements</span></span>

<span data-ttu-id="d631c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d631c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d631c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d631c-112">Parent elements</span></span>

|<span data-ttu-id="d631c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d631c-113">**Element**</span></span>|<span data-ttu-id="d631c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d631c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d631c-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="d631c-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="d631c-116">Spécifie des informations sur la licence de gestion des droits.</span><span class="sxs-lookup"><span data-stu-id="d631c-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d631c-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d631c-117">Text value</span></span>

<span data-ttu-id="d631c-118">Une valeur de texte de **la valeur true** pour l’élément **IsOwner** indique que l’utilisateur est le propriétaire des droits émis sur un élément.</span><span class="sxs-lookup"><span data-stu-id="d631c-118">A text value of **true** for the **IsOwner** element indicates that the user is the owner of rights issued on an item.</span></span> <span data-ttu-id="d631c-119">La valeur **false** indique que l’utilisateur n’est pas le propriétaire des droits émis sur un élément.</span><span class="sxs-lookup"><span data-stu-id="d631c-119">A value of **false** indicates that the user is not the owner of rights issued on an item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d631c-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="d631c-120">Remarks</span></span>

<span data-ttu-id="d631c-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d631c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d631c-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d631c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d631c-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d631c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d631c-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d631c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d631c-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d631c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d631c-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d631c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d631c-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="d631c-127">Validation File</span></span>  <br/> |<span data-ttu-id="d631c-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d631c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d631c-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d631c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d631c-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d631c-130">See also</span></span>



- [<span data-ttu-id="d631c-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d631c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

