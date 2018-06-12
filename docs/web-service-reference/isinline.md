---
title: IsInline
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInline
api_type:
- schema
ms.assetid: 5e7712c8-372a-4a16-be64-360c5ff3961a
description: L’élément IsInline représente si la pièce jointe apparaît en ligne au sein d’un élément.
ms.openlocfilehash: f2f9093777a3914de067ef63827de6cf354fc12d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828042"
---
# <a name="isinline"></a><span data-ttu-id="52460-103">IsInline</span><span class="sxs-lookup"><span data-stu-id="52460-103">IsInline</span></span>

<span data-ttu-id="52460-104">L’élément **IsInline** représente si la pièce jointe apparaît en ligne au sein d’un élément.</span><span class="sxs-lookup"><span data-stu-id="52460-104">The **IsInline** element represents whether the attachment appears inline within an item.</span></span> 
  
```xml
<IsInline>true or false</IsInline>
```

 <span data-ttu-id="52460-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="52460-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52460-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="52460-106">Attributes and elements</span></span>

<span data-ttu-id="52460-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="52460-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52460-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="52460-108">Attributes</span></span>

<span data-ttu-id="52460-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="52460-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52460-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="52460-110">Child elements</span></span>

<span data-ttu-id="52460-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="52460-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="52460-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="52460-112">Parent elements</span></span>

|<span data-ttu-id="52460-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="52460-113">**Element**</span></span>|<span data-ttu-id="52460-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="52460-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52460-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="52460-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="52460-116">Représente un fichier qui est attaché à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="52460-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="52460-117">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="52460-117">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="52460-118">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="52460-118">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="52460-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="52460-119">Text value</span></span>

<span data-ttu-id="52460-120">Cet élément peut être **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="52460-120">This element can be either **true** or **false**.</span></span> <span data-ttu-id="52460-121">La valeur par défaut est **false**.</span><span class="sxs-lookup"><span data-stu-id="52460-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="52460-122">Note</span><span class="sxs-lookup"><span data-stu-id="52460-122">Remarks</span></span>

<span data-ttu-id="52460-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="52460-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52460-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="52460-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52460-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="52460-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52460-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="52460-126">Schema Name</span></span>  <br/> |<span data-ttu-id="52460-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="52460-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="52460-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="52460-128">Validation File</span></span>  <br/> |<span data-ttu-id="52460-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="52460-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="52460-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="52460-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="52460-131">False</span><span class="sxs-lookup"><span data-stu-id="52460-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52460-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="52460-132">See also</span></span>



- [<span data-ttu-id="52460-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="52460-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

