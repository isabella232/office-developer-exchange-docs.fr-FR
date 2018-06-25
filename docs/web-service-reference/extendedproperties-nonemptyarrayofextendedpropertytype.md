---
title: ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a7034730-210d-4916-b992-dda342f890f8
description: L’élément ExtendedProperties spécifie un tableau de propriétés supplémentaires.
ms.openlocfilehash: b92108ecde63d4a3ac3cc80861c204c4d1950cc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756296"
---
# <a name="extendedproperties-nonemptyarrayofextendedpropertytype"></a><span data-ttu-id="7a4c8-103">ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="7a4c8-103">ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span></span>

<span data-ttu-id="7a4c8-104">L’élément **ExtendedProperties** spécifie un tableau de propriétés supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="7a4c8-104">The **ExtendedProperties** element specifies an array of additional properties.</span></span> 
  
```XML
<ExtendedProperties>
    <ExtendedProperty/>
</ExtendedProperties>
```

 <span data-ttu-id="7a4c8-105">**NonEmptyArrayOfExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="7a4c8-105">**NonEmptyArrayOfExtendedPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a4c8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7a4c8-106">Attributes and elements</span></span>

<span data-ttu-id="7a4c8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7a4c8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a4c8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7a4c8-108">Attributes</span></span>

<span data-ttu-id="7a4c8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7a4c8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a4c8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7a4c8-110">Child elements</span></span>

|<span data-ttu-id="7a4c8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a4c8-111">**Element**</span></span>|<span data-ttu-id="7a4c8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a4c8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a4c8-113">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="7a4c8-113">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="7a4c8-114">Identifie les propriétés MAPI étendues sur les dossiers et éléments.</span><span class="sxs-lookup"><span data-stu-id="7a4c8-114">Identifies extended MAPI properties on folders and items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a4c8-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7a4c8-115">Parent elements</span></span>

|<span data-ttu-id="7a4c8-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a4c8-116">**Element**</span></span>|<span data-ttu-id="7a4c8-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a4c8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a4c8-118">ImGroup</span><span class="sxs-lookup"><span data-stu-id="7a4c8-118">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="7a4c8-119">Représente un groupe de messagerie instantané.</span><span class="sxs-lookup"><span data-stu-id="7a4c8-119">Represents an instant messaging group.</span></span>  <br/> |
|[<span data-ttu-id="7a4c8-120">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="7a4c8-120">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="7a4c8-121">Spécifie les 256 premiers caractères d’un élément de boîte aux lettres pour l’aperçu sans ouvrir l’élément.</span><span class="sxs-lookup"><span data-stu-id="7a4c8-121">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a4c8-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="7a4c8-122">Remarks</span></span>

<span data-ttu-id="7a4c8-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7a4c8-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7a4c8-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a4c8-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a4c8-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7a4c8-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a4c8-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7a4c8-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a4c8-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7a4c8-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7a4c8-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="7a4c8-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="7a4c8-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="7a4c8-129">Validation File</span></span>  <br/> |<span data-ttu-id="7a4c8-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a4c8-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a4c8-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7a4c8-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7a4c8-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7a4c8-132">See also</span></span>



- [<span data-ttu-id="7a4c8-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7a4c8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

