---
title: ContentType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentType
api_type:
- schema
ms.assetid: f91ff0df-0d8a-43ea-a188-d80f0e885f19
description: L’élément ContentType décrit le type de Multipurpose Internet Mail Extensions (MIME) du contenu des pièces jointes.
ms.openlocfilehash: 489df47343051623d5b6a98557f2bd434a5dad52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755629"
---
# <a name="contenttype"></a><span data-ttu-id="44a9a-103">ContentType</span><span class="sxs-lookup"><span data-stu-id="44a9a-103">ContentType</span></span>

<span data-ttu-id="44a9a-104">L’élément **ContentType** décrit le type de Multipurpose Internet Mail Extensions (MIME) du contenu des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="44a9a-104">The **ContentType** element describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span> 
  
```xml
<ContentType/>
```

 <span data-ttu-id="44a9a-105">**Chaîne**</span><span class="sxs-lookup"><span data-stu-id="44a9a-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44a9a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="44a9a-106">Attributes and elements</span></span>

<span data-ttu-id="44a9a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="44a9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44a9a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="44a9a-108">Attributes</span></span>

<span data-ttu-id="44a9a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="44a9a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44a9a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="44a9a-110">Child elements</span></span>

<span data-ttu-id="44a9a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="44a9a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="44a9a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="44a9a-112">Parent elements</span></span>

|<span data-ttu-id="44a9a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="44a9a-113">**Element**</span></span>|<span data-ttu-id="44a9a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="44a9a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44a9a-115">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="44a9a-115">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="44a9a-116">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="44a9a-116">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="44a9a-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="44a9a-117">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="44a9a-118">Représente un fichier qui est attaché à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="44a9a-118">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="44a9a-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="44a9a-119">Text value</span></span>

<span data-ttu-id="44a9a-120">La valeur de texte est une valeur de type string qui représente le type de contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="44a9a-120">The text value is a string value that represents the content type of the attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="44a9a-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="44a9a-121">Remarks</span></span>

<span data-ttu-id="44a9a-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="44a9a-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44a9a-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="44a9a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44a9a-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="44a9a-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44a9a-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="44a9a-125">Schema name</span></span>  <br/> |<span data-ttu-id="44a9a-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="44a9a-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="44a9a-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="44a9a-127">Validation file</span></span>  <br/> |<span data-ttu-id="44a9a-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="44a9a-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="44a9a-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="44a9a-129">Can be empty</span></span>  <br/> |<span data-ttu-id="44a9a-130">False</span><span class="sxs-lookup"><span data-stu-id="44a9a-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44a9a-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="44a9a-131">See also</span></span>



- [<span data-ttu-id="44a9a-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="44a9a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

