---
title: IsManagedFoldersRoot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsManagedFoldersRoot
api_type:
- schema
ms.assetid: 00823fb9-bf8b-49bb-8e1b-d698c6d4063f
description: L’élément IsManagedFoldersRoot indique si le dossier géré est la racine de tous les dossiers gérés.
ms.openlocfilehash: 3484a3fef56545a9a8d56af65f56f75205918ec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828044"
---
# <a name="ismanagedfoldersroot"></a><span data-ttu-id="1d090-103">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="1d090-103">IsManagedFoldersRoot</span></span>

<span data-ttu-id="1d090-104">L’élément **IsManagedFoldersRoot** indique si le dossier géré est la racine de tous les dossiers gérés.</span><span class="sxs-lookup"><span data-stu-id="1d090-104">The **IsManagedFoldersRoot** element indicates whether the managed folder is the root for all managed folders.</span></span> 
  
```xml
<IsManagedFoldersRoot/>
```

 <span data-ttu-id="1d090-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1d090-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d090-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1d090-106">Attributes and elements</span></span>

<span data-ttu-id="1d090-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1d090-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d090-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1d090-108">Attributes</span></span>

<span data-ttu-id="1d090-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1d090-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d090-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1d090-110">Child elements</span></span>

<span data-ttu-id="1d090-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1d090-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1d090-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1d090-112">Parent elements</span></span>

|<span data-ttu-id="1d090-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1d090-113">**Element**</span></span>|<span data-ttu-id="1d090-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1d090-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d090-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="1d090-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="1d090-116">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="1d090-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1d090-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1d090-117">Text value</span></span>

<span data-ttu-id="1d090-118">Une valeur de texte qui représente une valeur Boolean est requise si cet élément est présent.</span><span class="sxs-lookup"><span data-stu-id="1d090-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="1d090-119">La valeur **true** indique que le dossier est le dossier racine du dossier géré. la valeur **false** indique que le dossier n’est pas le dossier racine du dossier géré.</span><span class="sxs-lookup"><span data-stu-id="1d090-119">A value of **true** indicates that the folder is the root folder of the managed folder; a value of **false** indicates that the folder is not the root folder of the managed folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1d090-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="1d090-120">Remarks</span></span>

<span data-ttu-id="1d090-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1d090-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d090-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1d090-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d090-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1d090-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1d090-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1d090-124">Schema name</span></span>  <br/> |<span data-ttu-id="1d090-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1d090-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="1d090-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1d090-126">Validation file</span></span>  <br/> |<span data-ttu-id="1d090-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1d090-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1d090-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1d090-128">Can be empty</span></span>  <br/> |<span data-ttu-id="1d090-129">False</span><span class="sxs-lookup"><span data-stu-id="1d090-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d090-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1d090-130">See also</span></span>



- [<span data-ttu-id="1d090-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1d090-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

