---
title: IsOwner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea0f0afc-32fe-46cb-8530-62a6ce9490f6
description: L’élément IsOwner spécifie si l’utilisateur de messagerie spécifié est le propriétaire.
ms.openlocfilehash: 2dd085aba34052d95efd1e72edca7be4aba71155
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466520"
---
# <a name="isowner"></a><span data-ttu-id="b5144-103">IsOwner</span><span class="sxs-lookup"><span data-stu-id="b5144-103">IsOwner</span></span>

<span data-ttu-id="b5144-104">L’élément **IsOwner** spécifie si l’utilisateur de messagerie spécifié est le propriétaire.</span><span class="sxs-lookup"><span data-stu-id="b5144-104">The **IsOwner** element specifies whether the specified email user is the owner.</span></span> 
  
```XML
<IsOwner>true | false</IsOwner>
```

 <span data-ttu-id="b5144-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b5144-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5144-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b5144-106">Attributes and elements</span></span>

<span data-ttu-id="b5144-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b5144-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5144-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b5144-108">Attributes</span></span>

<span data-ttu-id="b5144-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b5144-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5144-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b5144-110">Child elements</span></span>

<span data-ttu-id="b5144-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b5144-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5144-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b5144-112">Parent elements</span></span>

|<span data-ttu-id="b5144-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b5144-113">**Element**</span></span>|<span data-ttu-id="b5144-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b5144-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5144-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="b5144-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="b5144-116">Spécifie les informations relatives à la licence de gestion des droits.</span><span class="sxs-lookup"><span data-stu-id="b5144-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b5144-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="b5144-117">Text value</span></span>

<span data-ttu-id="b5144-118">Une valeur de texte de **true** pour l’élément **IsOwner** indique que l’utilisateur est le propriétaire de droits émis sur un élément.</span><span class="sxs-lookup"><span data-stu-id="b5144-118">A text value of **true** for the **IsOwner** element indicates that the user is the owner of rights issued on an item.</span></span> <span data-ttu-id="b5144-119">La valeur **false** indique que l’utilisateur n’est pas le propriétaire de droits émis sur un élément.</span><span class="sxs-lookup"><span data-stu-id="b5144-119">A value of **false** indicates that the user is not the owner of rights issued on an item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b5144-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="b5144-120">Remarks</span></span>

<span data-ttu-id="b5144-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b5144-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b5144-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5144-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5144-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b5144-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5144-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b5144-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5144-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b5144-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b5144-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="b5144-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b5144-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="b5144-127">Validation File</span></span>  <br/> |<span data-ttu-id="b5144-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="b5144-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5144-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b5144-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b5144-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b5144-130">See also</span></span>



- [<span data-ttu-id="b5144-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b5144-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

