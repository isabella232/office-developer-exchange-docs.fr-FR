---
title: HasQuota
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasQuota
api_type:
- schema
ms.assetid: b6e4fef0-92a9-415f-81ae-0c5ecb7c12ad
description: L’élément HasQuota indique si le dossier géré a un quota.
ms.openlocfilehash: 26f14ee7c9d4de267733bca11f7884d1d391b3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827807"
---
# <a name="hasquota"></a><span data-ttu-id="7e7dd-103">HasQuota</span><span class="sxs-lookup"><span data-stu-id="7e7dd-103">HasQuota</span></span>

<span data-ttu-id="7e7dd-104">L’élément **HasQuota** indique si le dossier géré a un quota.</span><span class="sxs-lookup"><span data-stu-id="7e7dd-104">The **HasQuota** element indicates whether the managed folder has a quota.</span></span> 
  
```xml
<HasQuota/>
```

 <span data-ttu-id="7e7dd-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7e7dd-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e7dd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7e7dd-106">Attributes and elements</span></span>

<span data-ttu-id="7e7dd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7e7dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e7dd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7e7dd-108">Attributes</span></span>

<span data-ttu-id="7e7dd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7e7dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e7dd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7e7dd-110">Child elements</span></span>

<span data-ttu-id="7e7dd-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7e7dd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e7dd-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7e7dd-112">Parent elements</span></span>

|<span data-ttu-id="7e7dd-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7e7dd-113">**Element**</span></span>|<span data-ttu-id="7e7dd-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7e7dd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e7dd-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="7e7dd-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="7e7dd-116">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="7e7dd-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e7dd-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7e7dd-117">Text value</span></span>

<span data-ttu-id="7e7dd-118">La valeur de texte représente une valeur de type Boolean.</span><span class="sxs-lookup"><span data-stu-id="7e7dd-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="7e7dd-119">La valeur **true** indique que le dossier dispose d’un quota ; la valeur **false** indique que le dossier n’a pas de quota.</span><span class="sxs-lookup"><span data-stu-id="7e7dd-119">A value of **true** indicates that the folder has a quota; a value of **false** indicates that the folder does not have a quota.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7e7dd-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="7e7dd-120">Remarks</span></span>

<span data-ttu-id="7e7dd-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7e7dd-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e7dd-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7e7dd-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e7dd-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7e7dd-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e7dd-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7e7dd-124">Schema name</span></span>  <br/> |<span data-ttu-id="7e7dd-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7e7dd-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e7dd-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7e7dd-126">Validation file</span></span>  <br/> |<span data-ttu-id="7e7dd-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e7dd-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e7dd-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7e7dd-128">Can be empty</span></span>  <br/> |<span data-ttu-id="7e7dd-129">False</span><span class="sxs-lookup"><span data-stu-id="7e7dd-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e7dd-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7e7dd-130">See also</span></span>



- [<span data-ttu-id="7e7dd-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7e7dd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

