---
title: Content
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Content
api_type:
- schema
ms.assetid: 24f8c54a-505f-4fc0-b7e7-93ad50b97070
description: L’élément de contenu contient le contenu d’une pièce jointe codée en Base64.
ms.openlocfilehash: 20afe6286d3efaa5da6cdc88e397e88fddb1d8c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755614"
---
# <a name="content"></a><span data-ttu-id="d04ed-103">Content</span><span class="sxs-lookup"><span data-stu-id="d04ed-103">Content</span></span>

<span data-ttu-id="d04ed-104">L’élément de **contenu** contient le contenu d’une pièce jointe codée en Base64.</span><span class="sxs-lookup"><span data-stu-id="d04ed-104">The **Content** element contains the Base64-encoded contents of a file attachment.</span></span> 
  
```xml
<Content/>
```

 <span data-ttu-id="d04ed-105">**Base64Binary**</span><span class="sxs-lookup"><span data-stu-id="d04ed-105">**Base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d04ed-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d04ed-106">Attributes and elements</span></span>

<span data-ttu-id="d04ed-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d04ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d04ed-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d04ed-108">Attributes</span></span>

<span data-ttu-id="d04ed-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d04ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d04ed-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d04ed-110">Child elements</span></span>

<span data-ttu-id="d04ed-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d04ed-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d04ed-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d04ed-112">Parent elements</span></span>

|<span data-ttu-id="d04ed-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d04ed-113">**Element**</span></span>|<span data-ttu-id="d04ed-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d04ed-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d04ed-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="d04ed-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="d04ed-116">Représente un fichier t est thattached à un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="d04ed-116">Represents a file t is thattached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d04ed-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d04ed-117">Text value</span></span>

<span data-ttu-id="d04ed-118">La valeur de chaîne représente les données binaires de la pièce jointe codée en Base64.</span><span class="sxs-lookup"><span data-stu-id="d04ed-118">The string value represents the Base64-encoded binary data of the file attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d04ed-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="d04ed-119">Remarks</span></span>

<span data-ttu-id="d04ed-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d04ed-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d04ed-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d04ed-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d04ed-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d04ed-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d04ed-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d04ed-123">Schema name</span></span>  <br/> |<span data-ttu-id="d04ed-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d04ed-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="d04ed-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d04ed-125">Validation file</span></span>  <br/> |<span data-ttu-id="d04ed-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d04ed-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d04ed-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d04ed-127">Can be empty</span></span>  <br/> |<span data-ttu-id="d04ed-128">False</span><span class="sxs-lookup"><span data-stu-id="d04ed-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d04ed-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d04ed-129">See also</span></span>



- [<span data-ttu-id="d04ed-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d04ed-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

