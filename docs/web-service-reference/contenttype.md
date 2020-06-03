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
description: L’élément ContentType décrit le type MIME (Multipurpose Internet Mail Extensions) du contenu de la pièce jointe.
ms.openlocfilehash: cb326bb761ea28e0e9f77501bf754c7c1f0318fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455225"
---
# <a name="contenttype"></a><span data-ttu-id="ddbeb-103">ContentType</span><span class="sxs-lookup"><span data-stu-id="ddbeb-103">ContentType</span></span>

<span data-ttu-id="ddbeb-104">L’élément **ContentType** décrit le type MIME (Multipurpose Internet Mail Extensions) du contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-104">The **ContentType** element describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span> 
  
```xml
<ContentType/>
```

 <span data-ttu-id="ddbeb-105">**String**</span><span class="sxs-lookup"><span data-stu-id="ddbeb-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ddbeb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ddbeb-106">Attributes and elements</span></span>

<span data-ttu-id="ddbeb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ddbeb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ddbeb-108">Attributes</span></span>

<span data-ttu-id="ddbeb-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ddbeb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ddbeb-110">Child elements</span></span>

<span data-ttu-id="ddbeb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ddbeb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ddbeb-112">Parent elements</span></span>

|<span data-ttu-id="ddbeb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ddbeb-113">**Element**</span></span>|<span data-ttu-id="ddbeb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ddbeb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddbeb-115">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ddbeb-115">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="ddbeb-116">Représente un élément Exchange qui est joint à un autre élément Exchange.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-116">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="ddbeb-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="ddbeb-117">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="ddbeb-118">Représente un fichier joint à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-118">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ddbeb-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ddbeb-119">Text value</span></span>

<span data-ttu-id="ddbeb-120">La valeur de texte est une valeur de chaîne qui représente le type de contenu de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-120">The text value is a string value that represents the content type of the attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ddbeb-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="ddbeb-121">Remarks</span></span>

<span data-ttu-id="ddbeb-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ddbeb-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ddbeb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ddbeb-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ddbeb-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ddbeb-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ddbeb-125">Schema name</span></span>  <br/> |<span data-ttu-id="ddbeb-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ddbeb-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="ddbeb-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ddbeb-127">Validation file</span></span>  <br/> |<span data-ttu-id="ddbeb-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ddbeb-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ddbeb-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ddbeb-129">Can be empty</span></span>  <br/> |<span data-ttu-id="ddbeb-130">False</span><span class="sxs-lookup"><span data-stu-id="ddbeb-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ddbeb-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ddbeb-131">See also</span></span>



- [<span data-ttu-id="ddbeb-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ddbeb-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

