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
description: L’élément CanRenameOrMove indique si un dossier géré permettre être renommé ou déplacé par le client.
ms.openlocfilehash: 0303499f5cd54d4a52222e43c2c5f0b389fbcf53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755497"
---
# <a name="canrenameormove"></a><span data-ttu-id="71204-103">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="71204-103">CanRenameOrMove</span></span>

<span data-ttu-id="71204-104">L’élément **CanRenameOrMove** indique si un dossier géré permettre être renommé ou déplacé par le client.</span><span class="sxs-lookup"><span data-stu-id="71204-104">The **CanRenameOrMove** element indicates whether a managed folder can be renamed or moved by the customer.</span></span> 
  
```xml
<CanRenameOrMove/>
```

 <span data-ttu-id="71204-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="71204-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71204-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="71204-106">Attributes and elements</span></span>

<span data-ttu-id="71204-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="71204-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71204-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="71204-108">Attributes</span></span>

<span data-ttu-id="71204-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="71204-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71204-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="71204-110">Child elements</span></span>

<span data-ttu-id="71204-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="71204-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="71204-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="71204-112">Parent elements</span></span>

|<span data-ttu-id="71204-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71204-113">**Element**</span></span>|<span data-ttu-id="71204-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="71204-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71204-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="71204-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="71204-116">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="71204-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="71204-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="71204-117">Text value</span></span>

<span data-ttu-id="71204-118">La valeur de texte représente une valeur de type Boolean.</span><span class="sxs-lookup"><span data-stu-id="71204-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="71204-119">La valeur **true** indique que le dossier peut être renommé ou déplacé ; la valeur **false** indique que le dossier ne peut pas être renommé ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="71204-119">A value of **true** indicates that the folder can be renamed or moved; a value of **false** indicates that the folder cannot be renamed or moved.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="71204-120">Note</span><span class="sxs-lookup"><span data-stu-id="71204-120">Remarks</span></span>

<span data-ttu-id="71204-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="71204-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71204-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="71204-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71204-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="71204-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71204-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="71204-124">Schema name</span></span>  <br/> |<span data-ttu-id="71204-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="71204-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="71204-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="71204-126">Validation file</span></span>  <br/> |<span data-ttu-id="71204-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71204-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71204-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="71204-128">Can be empty</span></span>  <br/> |<span data-ttu-id="71204-129">False</span><span class="sxs-lookup"><span data-stu-id="71204-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71204-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="71204-130">See also</span></span>



- [<span data-ttu-id="71204-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="71204-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

