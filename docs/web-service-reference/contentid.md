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
description: L’élément ContentId représente un identificateur pour le contenu d’une pièce jointe. ContentId peut être définie à n’importe quelle valeur de chaîne. Applications peuvent utiliser ContentId pour implémenter leurs propres mécanismes d’identification.
ms.openlocfilehash: dc46ae4b33d435f5d47eb7deb39e92fd0170194b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755621"
---
# <a name="contentid"></a><span data-ttu-id="456e2-105">ContentId</span><span class="sxs-lookup"><span data-stu-id="456e2-105">ContentId</span></span>

<span data-ttu-id="456e2-106">L’élément **ContentId** représente un identificateur pour le contenu d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="456e2-106">The **ContentId** element represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="456e2-107">**ContentId** peut être définie à n’importe quelle valeur de chaîne.</span><span class="sxs-lookup"><span data-stu-id="456e2-107">**ContentId** can be set to any string value.</span></span> <span data-ttu-id="456e2-108">Applications peuvent utiliser **ContentId** pour implémenter leurs propres mécanismes d’identification.</span><span class="sxs-lookup"><span data-stu-id="456e2-108">Applications can use **ContentId** to implement their own identification mechanisms.</span></span> 
  
```xml
<ContentId/>
```

 <span data-ttu-id="456e2-109">**Chaîne**</span><span class="sxs-lookup"><span data-stu-id="456e2-109">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="456e2-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="456e2-110">Attributes and elements</span></span>

<span data-ttu-id="456e2-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="456e2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="456e2-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="456e2-112">Attributes</span></span>

<span data-ttu-id="456e2-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="456e2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="456e2-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="456e2-114">Child elements</span></span>

<span data-ttu-id="456e2-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="456e2-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="456e2-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="456e2-116">Parent elements</span></span>

|<span data-ttu-id="456e2-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="456e2-117">**Element**</span></span>|<span data-ttu-id="456e2-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="456e2-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="456e2-119">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="456e2-119">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="456e2-120">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="456e2-120">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="456e2-121">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="456e2-121">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="456e2-122">Représente un fichier qui est attaché à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="456e2-122">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="456e2-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="456e2-123">Text value</span></span>

<span data-ttu-id="456e2-124">La valeur de chaîne représente l’identificateur pour le contenu d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="456e2-124">The string value represents the identifier to the contents of an attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="456e2-125">Note</span><span class="sxs-lookup"><span data-stu-id="456e2-125">Remarks</span></span>

<span data-ttu-id="456e2-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="456e2-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="456e2-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="456e2-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="456e2-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="456e2-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="456e2-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="456e2-129">Schema name</span></span>  <br/> |<span data-ttu-id="456e2-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="456e2-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="456e2-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="456e2-131">Validation file</span></span>  <br/> |<span data-ttu-id="456e2-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="456e2-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="456e2-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="456e2-133">Can be empty</span></span>  <br/> |<span data-ttu-id="456e2-134">False</span><span class="sxs-lookup"><span data-stu-id="456e2-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="456e2-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="456e2-135">See also</span></span>



- [<span data-ttu-id="456e2-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="456e2-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

