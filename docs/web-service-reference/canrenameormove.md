---
title: CanRenameOrMove
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanRenameOrMove
api_type:
- schema
ms.assetid: fe0cdb04-5f2b-4f1d-9d12-7ace0883cd86
description: L’élément CanRenameOrMove indique si un dossier géré peut être renommé ou déplacé par le client.
ms.openlocfilehash: eb6aaeb8b0edcab5b67212c426a44daf32a0cf73
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463362"
---
# <a name="canrenameormove"></a><span data-ttu-id="dcae2-103">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="dcae2-103">CanRenameOrMove</span></span>

<span data-ttu-id="dcae2-104">L’élément **CanRenameOrMove** indique si un dossier géré peut être renommé ou déplacé par le client.</span><span class="sxs-lookup"><span data-stu-id="dcae2-104">The **CanRenameOrMove** element indicates whether a managed folder can be renamed or moved by the customer.</span></span> 
  
```xml
<CanRenameOrMove/>
```

 <span data-ttu-id="dcae2-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="dcae2-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dcae2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dcae2-106">Attributes and elements</span></span>

<span data-ttu-id="dcae2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dcae2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcae2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dcae2-108">Attributes</span></span>

<span data-ttu-id="dcae2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="dcae2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dcae2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dcae2-110">Child elements</span></span>

<span data-ttu-id="dcae2-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dcae2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dcae2-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dcae2-112">Parent elements</span></span>

|<span data-ttu-id="dcae2-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dcae2-113">**Element**</span></span>|<span data-ttu-id="dcae2-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="dcae2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcae2-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="dcae2-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="dcae2-116">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="dcae2-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dcae2-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="dcae2-117">Text value</span></span>

<span data-ttu-id="dcae2-118">La valeur de texte représente une valeur de type Boolean.</span><span class="sxs-lookup"><span data-stu-id="dcae2-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="dcae2-119">La valeur **true** indique que le dossier peut être renommé ou déplacé ; la valeur **false** indique que le dossier ne peut pas être renommé ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="dcae2-119">A value of **true** indicates that the folder can be renamed or moved; a value of **false** indicates that the folder cannot be renamed or moved.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="dcae2-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="dcae2-120">Remarks</span></span>

<span data-ttu-id="dcae2-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="dcae2-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dcae2-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dcae2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcae2-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dcae2-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dcae2-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dcae2-124">Schema name</span></span>  <br/> |<span data-ttu-id="dcae2-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="dcae2-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="dcae2-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dcae2-126">Validation file</span></span>  <br/> |<span data-ttu-id="dcae2-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dcae2-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dcae2-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dcae2-128">Can be empty</span></span>  <br/> |<span data-ttu-id="dcae2-129">False</span><span class="sxs-lookup"><span data-stu-id="dcae2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dcae2-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dcae2-130">See also</span></span>



- [<span data-ttu-id="dcae2-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dcae2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

