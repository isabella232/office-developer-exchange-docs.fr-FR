---
title: ContentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentId
api_type:
- schema
ms.assetid: bc59100d-6079-414b-a6e0-7c15feaa3184
description: L’élément ContentId représente un identificateur pour le contenu d’une pièce jointe. ContentId peut être défini sur n’importe quelle valeur de chaîne. Les applications peuvent utiliser ContentId pour implémenter leurs propres mécanismes d’identification.
ms.openlocfilehash: ca89c8790e839326412003f26b738ad1ee956211
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529265"
---
# <a name="contentid"></a><span data-ttu-id="3e54d-105">ContentId</span><span class="sxs-lookup"><span data-stu-id="3e54d-105">ContentId</span></span>

<span data-ttu-id="3e54d-106">L’élément **contentid** représente un identificateur pour le contenu d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="3e54d-106">The **ContentId** element represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="3e54d-107">**Contentid** peut être défini sur n’importe quelle valeur de chaîne.</span><span class="sxs-lookup"><span data-stu-id="3e54d-107">**ContentId** can be set to any string value.</span></span> <span data-ttu-id="3e54d-108">Les applications peuvent utiliser **contentid** pour implémenter leurs propres mécanismes d’identification.</span><span class="sxs-lookup"><span data-stu-id="3e54d-108">Applications can use **ContentId** to implement their own identification mechanisms.</span></span> 
  
```xml
<ContentId/>
```

 <span data-ttu-id="3e54d-109">**String**</span><span class="sxs-lookup"><span data-stu-id="3e54d-109">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e54d-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3e54d-110">Attributes and elements</span></span>

<span data-ttu-id="3e54d-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3e54d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e54d-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="3e54d-112">Attributes</span></span>

<span data-ttu-id="3e54d-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3e54d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e54d-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3e54d-114">Child elements</span></span>

<span data-ttu-id="3e54d-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3e54d-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3e54d-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3e54d-116">Parent elements</span></span>

|<span data-ttu-id="3e54d-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e54d-117">**Element**</span></span>|<span data-ttu-id="3e54d-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e54d-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e54d-119">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="3e54d-119">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="3e54d-120">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e54d-120">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="3e54d-121">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="3e54d-121">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="3e54d-122">Représente un fichier joint à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e54d-122">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3e54d-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="3e54d-123">Text value</span></span>

<span data-ttu-id="3e54d-124">La valeur de chaîne représente l’identificateur du contenu d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="3e54d-124">The string value represents the identifier to the contents of an attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3e54d-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="3e54d-125">Remarks</span></span>

<span data-ttu-id="3e54d-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3e54d-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e54d-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3e54d-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e54d-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3e54d-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3e54d-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3e54d-129">Schema name</span></span>  <br/> |<span data-ttu-id="3e54d-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3e54d-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="3e54d-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3e54d-131">Validation file</span></span>  <br/> |<span data-ttu-id="3e54d-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3e54d-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3e54d-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3e54d-133">Can be empty</span></span>  <br/> |<span data-ttu-id="3e54d-134">False</span><span class="sxs-lookup"><span data-stu-id="3e54d-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e54d-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3e54d-135">See also</span></span>



- [<span data-ttu-id="3e54d-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3e54d-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

