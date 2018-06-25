---
title: HasAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: L’élément HasAttachment spécifie une valeur booléenne pour indiquer si l’élément a des pièces jointes.
ms.openlocfilehash: dfe163e0850e835784a43984a34c89f14bfbc59b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827798"
---
# <a name="hasattachment"></a><span data-ttu-id="a6bcf-103">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="a6bcf-103">HasAttachment</span></span>

<span data-ttu-id="a6bcf-104">L’élément **HasAttachment** spécifie une valeur booléenne pour indiquer si l’élément a des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="a6bcf-104">The **HasAttachment** element specifies a Boolean value to indicate whether the item has attachments.</span></span> 
  
```XML
<HasAttachment> true | false </HasAttachment
```

 <span data-ttu-id="a6bcf-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a6bcf-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6bcf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a6bcf-106">Attributes and elements</span></span>

<span data-ttu-id="a6bcf-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a6bcf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6bcf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a6bcf-108">Attributes</span></span>

<span data-ttu-id="a6bcf-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a6bcf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a6bcf-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a6bcf-110">Child elements</span></span>

<span data-ttu-id="a6bcf-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a6bcf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a6bcf-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a6bcf-112">Parent elements</span></span>

|<span data-ttu-id="a6bcf-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a6bcf-113">**Element**</span></span>|<span data-ttu-id="a6bcf-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a6bcf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6bcf-115">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="a6bcf-115">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="a6bcf-116">Spécifie les 256 premiers caractères d’un élément de boîte aux lettres pour l’aperçu sans ouvrir l’élément.</span><span class="sxs-lookup"><span data-stu-id="a6bcf-116">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a6bcf-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a6bcf-117">Text value</span></span>

<span data-ttu-id="a6bcf-118">Une valeur de texte de **la valeur true** pour l’élément **HasAttachment** indique qu’une pièce jointe à l’élément.</span><span class="sxs-lookup"><span data-stu-id="a6bcf-118">A text value of **true** for the **HasAttachment** element indicates that the item has an attachment.</span></span> <span data-ttu-id="a6bcf-119">La valeur **false** indique que l’élément ne dispose pas d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="a6bcf-119">A value of **false** indicates that the item does not have an attachment.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a6bcf-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="a6bcf-120">Remarks</span></span>

<span data-ttu-id="a6bcf-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a6bcf-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a6bcf-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a6bcf-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6bcf-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a6bcf-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6bcf-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a6bcf-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a6bcf-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a6bcf-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a6bcf-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="a6bcf-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="a6bcf-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="a6bcf-127">Validation File</span></span>  <br/> |<span data-ttu-id="a6bcf-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="a6bcf-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a6bcf-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a6bcf-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a6bcf-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a6bcf-130">See also</span></span>



- [<span data-ttu-id="a6bcf-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a6bcf-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

