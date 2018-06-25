---
title: FolderChanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChanges
api_type:
- schema
ms.assetid: d3f611ed-56a4-43f8-aa65-cbd7844b827f
description: L’élément FolderChanges représente une collection des modifications pour un dossier.
ms.openlocfilehash: 7ab89e79f6babb5e93863974835685c6975d96dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756437"
---
# <a name="folderchanges"></a><span data-ttu-id="9a018-103">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="9a018-103">FolderChanges</span></span>

<span data-ttu-id="9a018-104">L’élément **FolderChanges** représente une collection des modifications pour un dossier.</span><span class="sxs-lookup"><span data-stu-id="9a018-104">The **FolderChanges** element represents a collection of changes for a folder.</span></span> 
  
[<span data-ttu-id="9a018-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="9a018-105">UpdateFolder</span></span>](updatefolder.md)
  
[<span data-ttu-id="9a018-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="9a018-106">FolderChanges</span></span>](folderchanges.md)
  
```xml
<FolderChanges>
   <FolderChange/>
</FolderChanges>
```

 <span data-ttu-id="9a018-107">**NonEmptyArrayOfFolderChangesType**</span><span class="sxs-lookup"><span data-stu-id="9a018-107">**NonEmptyArrayOfFolderChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a018-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9a018-108">Attributes and elements</span></span>

<span data-ttu-id="9a018-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9a018-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a018-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="9a018-110">Attributes</span></span>

<span data-ttu-id="9a018-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a018-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a018-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9a018-112">Child elements</span></span>

|<span data-ttu-id="9a018-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a018-113">**Element**</span></span>|<span data-ttu-id="9a018-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a018-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a018-115">FolderChange</span><span class="sxs-lookup"><span data-stu-id="9a018-115">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="9a018-116">Représente une modification à effectuer sur un seul dossier unique.</span><span class="sxs-lookup"><span data-stu-id="9a018-116">Represents a single change to be performed on a single folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a018-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9a018-117">Parent elements</span></span>

|<span data-ttu-id="9a018-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a018-118">**Element**</span></span>|<span data-ttu-id="9a018-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a018-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a018-120">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="9a018-120">UpdateFolder</span></span>](updatefolder.md) <br/> |<span data-ttu-id="9a018-121">Représente l’opération qui sert à mettre à jour les propriétés d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="9a018-121">Represents the operation that is used to update properties for a folder.</span></span>  <br/> <span data-ttu-id="9a018-122">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="9a018-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9a018-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="9a018-123">Remarks</span></span>

<span data-ttu-id="9a018-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9a018-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a018-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9a018-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a018-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9a018-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9a018-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9a018-127">Schema Name</span></span>  <br/> |<span data-ttu-id="9a018-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9a018-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9a018-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9a018-129">Validation File</span></span>  <br/> |<span data-ttu-id="9a018-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9a018-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9a018-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9a018-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a018-132">False</span><span class="sxs-lookup"><span data-stu-id="9a018-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a018-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9a018-133">See also</span></span>



[<span data-ttu-id="9a018-134">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="9a018-134">UpdateFolder operation</span></span>](updatefolder-operation.md)

