---
title: EditAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e63c4f7e-77c0-4826-b4e2-43b795d03914
description: L’élément EditAllowed spécifie si la gestion des droits relatifs à l’information peut être modifiée.
ms.openlocfilehash: 979fbaa9fcfbd1015468a8ae00628959bad0bf56
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463481"
---
# <a name="editallowed"></a><span data-ttu-id="79c68-103">EditAllowed</span><span class="sxs-lookup"><span data-stu-id="79c68-103">EditAllowed</span></span>

<span data-ttu-id="79c68-104">L’élément **EditAllowed** spécifie si la gestion des droits relatifs à l’information peut être modifiée.</span><span class="sxs-lookup"><span data-stu-id="79c68-104">The **EditAllowed** element specifies whether Information Rights Management can be edited.</span></span> 
  
```XML
<EditAllowed> true | false </EditAllowed>
```

 <span data-ttu-id="79c68-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="79c68-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79c68-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="79c68-106">Attributes and elements</span></span>

<span data-ttu-id="79c68-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="79c68-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79c68-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="79c68-108">Attributes</span></span>

<span data-ttu-id="79c68-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="79c68-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79c68-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="79c68-110">Child elements</span></span>

<span data-ttu-id="79c68-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79c68-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79c68-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="79c68-112">Parent elements</span></span>

|<span data-ttu-id="79c68-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79c68-113">**Element**</span></span>|<span data-ttu-id="79c68-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="79c68-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79c68-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="79c68-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="79c68-116">Spécifie les informations relatives à la licence de gestion des droits.</span><span class="sxs-lookup"><span data-stu-id="79c68-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79c68-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="79c68-117">Text value</span></span>

<span data-ttu-id="79c68-118">Une valeur de texte de **true** pour l’élément **EditAllowed** indique que la gestion des droits relatifs à l’information (IRM) peut être modifiée.</span><span class="sxs-lookup"><span data-stu-id="79c68-118">A text value of **true** for the **EditAllowed** element indicates that Information Rights Management (IRM) can be edited.</span></span> <span data-ttu-id="79c68-119">La valeur **false** indique qu’IRM ne peut pas être modifié.</span><span class="sxs-lookup"><span data-stu-id="79c68-119">A value of **false** indicates that IRM cannot be edited.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="79c68-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="79c68-120">Remarks</span></span>

<span data-ttu-id="79c68-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="79c68-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="79c68-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="79c68-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79c68-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="79c68-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79c68-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="79c68-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79c68-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="79c68-125">Schema Name</span></span>  <br/> |<span data-ttu-id="79c68-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="79c68-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="79c68-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="79c68-127">Validation File</span></span>  <br/> |<span data-ttu-id="79c68-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="79c68-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="79c68-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="79c68-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="79c68-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79c68-130">See also</span></span>



- [<span data-ttu-id="79c68-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="79c68-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

