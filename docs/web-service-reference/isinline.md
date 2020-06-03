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
description: L’élément IsInline indique si la pièce jointe s’affiche en ligne dans un élément.
ms.openlocfilehash: 2b3b6392fe8867ae9782dcb7211c17f4f4d9becd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464209"
---
# <a name="isinline"></a><span data-ttu-id="809d7-103">IsInline</span><span class="sxs-lookup"><span data-stu-id="809d7-103">IsInline</span></span>

<span data-ttu-id="809d7-104">L’élément **IsInline** indique si la pièce jointe s’affiche en ligne dans un élément.</span><span class="sxs-lookup"><span data-stu-id="809d7-104">The **IsInline** element represents whether the attachment appears inline within an item.</span></span> 
  
```xml
<IsInline>true or false</IsInline>
```

 <span data-ttu-id="809d7-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="809d7-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="809d7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="809d7-106">Attributes and elements</span></span>

<span data-ttu-id="809d7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="809d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="809d7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="809d7-108">Attributes</span></span>

<span data-ttu-id="809d7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="809d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="809d7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="809d7-110">Child elements</span></span>

<span data-ttu-id="809d7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="809d7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="809d7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="809d7-112">Parent elements</span></span>

|<span data-ttu-id="809d7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="809d7-113">**Element**</span></span>|<span data-ttu-id="809d7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="809d7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="809d7-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="809d7-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="809d7-116">Représente un fichier joint à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="809d7-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="809d7-117">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="809d7-117">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="809d7-118">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="809d7-118">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="809d7-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="809d7-119">Text value</span></span>

<span data-ttu-id="809d7-120">Cet élément peut avoir la **valeur true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="809d7-120">This element can be either **true** or **false**.</span></span> <span data-ttu-id="809d7-121">La valeur par défaut est **false**.</span><span class="sxs-lookup"><span data-stu-id="809d7-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="809d7-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="809d7-122">Remarks</span></span>

<span data-ttu-id="809d7-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="809d7-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="809d7-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="809d7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="809d7-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="809d7-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="809d7-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="809d7-126">Schema Name</span></span>  <br/> |<span data-ttu-id="809d7-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="809d7-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="809d7-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="809d7-128">Validation File</span></span>  <br/> |<span data-ttu-id="809d7-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="809d7-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="809d7-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="809d7-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="809d7-131">False</span><span class="sxs-lookup"><span data-stu-id="809d7-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="809d7-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="809d7-132">See also</span></span>



- [<span data-ttu-id="809d7-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="809d7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

