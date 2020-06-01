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
ms.openlocfilehash: 4373dba9dce92de8e175948d889f0806e100fa6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466023"
---
# <a name="ismanagedfoldersroot"></a><span data-ttu-id="66d00-103">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="66d00-103">IsManagedFoldersRoot</span></span>

<span data-ttu-id="66d00-104">L’élément **IsManagedFoldersRoot** indique si le dossier géré est la racine de tous les dossiers gérés.</span><span class="sxs-lookup"><span data-stu-id="66d00-104">The **IsManagedFoldersRoot** element indicates whether the managed folder is the root for all managed folders.</span></span> 
  
```xml
<IsManagedFoldersRoot/>
```

 <span data-ttu-id="66d00-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="66d00-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66d00-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="66d00-106">Attributes and elements</span></span>

<span data-ttu-id="66d00-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="66d00-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66d00-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="66d00-108">Attributes</span></span>

<span data-ttu-id="66d00-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="66d00-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66d00-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="66d00-110">Child elements</span></span>

<span data-ttu-id="66d00-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="66d00-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66d00-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="66d00-112">Parent elements</span></span>

|<span data-ttu-id="66d00-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="66d00-113">**Element**</span></span>|<span data-ttu-id="66d00-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="66d00-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66d00-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="66d00-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="66d00-116">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="66d00-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="66d00-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="66d00-117">Text value</span></span>

<span data-ttu-id="66d00-118">Une valeur de texte qui représente une valeur booléenne est requise si cet élément est présent.</span><span class="sxs-lookup"><span data-stu-id="66d00-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="66d00-119">La valeur **true** indique que le dossier est le dossier racine du dossier géré ; la valeur **false** indique que le dossier n’est pas le dossier racine du dossier géré.</span><span class="sxs-lookup"><span data-stu-id="66d00-119">A value of **true** indicates that the folder is the root folder of the managed folder; a value of **false** indicates that the folder is not the root folder of the managed folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="66d00-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="66d00-120">Remarks</span></span>

<span data-ttu-id="66d00-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="66d00-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66d00-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="66d00-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66d00-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="66d00-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="66d00-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="66d00-124">Schema name</span></span>  <br/> |<span data-ttu-id="66d00-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="66d00-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="66d00-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="66d00-126">Validation file</span></span>  <br/> |<span data-ttu-id="66d00-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="66d00-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="66d00-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="66d00-128">Can be empty</span></span>  <br/> |<span data-ttu-id="66d00-129">False</span><span class="sxs-lookup"><span data-stu-id="66d00-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66d00-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="66d00-130">See also</span></span>



- [<span data-ttu-id="66d00-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="66d00-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

