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
ms.openlocfilehash: 6e32aa4c69943774be928339936cca5016c58d85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462751"
---
# <a name="hasquota"></a><span data-ttu-id="8c418-103">HasQuota</span><span class="sxs-lookup"><span data-stu-id="8c418-103">HasQuota</span></span>

<span data-ttu-id="8c418-104">L’élément **HasQuota** indique si le dossier géré a un quota.</span><span class="sxs-lookup"><span data-stu-id="8c418-104">The **HasQuota** element indicates whether the managed folder has a quota.</span></span> 
  
```xml
<HasQuota/>
```

 <span data-ttu-id="8c418-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8c418-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8c418-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8c418-106">Attributes and elements</span></span>

<span data-ttu-id="8c418-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8c418-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c418-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8c418-108">Attributes</span></span>

<span data-ttu-id="8c418-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8c418-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8c418-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8c418-110">Child elements</span></span>

<span data-ttu-id="8c418-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8c418-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8c418-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8c418-112">Parent elements</span></span>

|<span data-ttu-id="8c418-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8c418-113">**Element**</span></span>|<span data-ttu-id="8c418-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="8c418-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c418-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="8c418-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="8c418-116">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="8c418-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8c418-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="8c418-117">Text value</span></span>

<span data-ttu-id="8c418-118">La valeur de texte représente une valeur de type Boolean.</span><span class="sxs-lookup"><span data-stu-id="8c418-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="8c418-119">La valeur **true** indique que le dossier a un quota ; la valeur **false** indique que le dossier ne possède pas de quota.</span><span class="sxs-lookup"><span data-stu-id="8c418-119">A value of **true** indicates that the folder has a quota; a value of **false** indicates that the folder does not have a quota.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8c418-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="8c418-120">Remarks</span></span>

<span data-ttu-id="8c418-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8c418-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8c418-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8c418-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8c418-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8c418-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8c418-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8c418-124">Schema name</span></span>  <br/> |<span data-ttu-id="8c418-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8c418-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8c418-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8c418-126">Validation file</span></span>  <br/> |<span data-ttu-id="8c418-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8c418-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8c418-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8c418-128">Can be empty</span></span>  <br/> |<span data-ttu-id="8c418-129">False</span><span class="sxs-lookup"><span data-stu-id="8c418-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8c418-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8c418-130">See also</span></span>



- [<span data-ttu-id="8c418-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8c418-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

