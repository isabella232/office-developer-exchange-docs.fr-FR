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
description: L’élément FolderChanges représente une collection de modifications apportées à un dossier.
ms.openlocfilehash: 5481496100512584fd0b9745ee42d5b9516bd7fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458382"
---
# <a name="folderchanges"></a><span data-ttu-id="76fff-103">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="76fff-103">FolderChanges</span></span>

<span data-ttu-id="76fff-104">L’élément **FolderChanges** représente une collection de modifications apportées à un dossier.</span><span class="sxs-lookup"><span data-stu-id="76fff-104">The **FolderChanges** element represents a collection of changes for a folder.</span></span> 
  
[<span data-ttu-id="76fff-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="76fff-105">UpdateFolder</span></span>](updatefolder.md)
  
[<span data-ttu-id="76fff-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="76fff-106">FolderChanges</span></span>](folderchanges.md)
  
```xml
<FolderChanges>
   <FolderChange/>
</FolderChanges>
```

 <span data-ttu-id="76fff-107">**NonEmptyArrayOfFolderChangesType**</span><span class="sxs-lookup"><span data-stu-id="76fff-107">**NonEmptyArrayOfFolderChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76fff-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="76fff-108">Attributes and elements</span></span>

<span data-ttu-id="76fff-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="76fff-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76fff-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="76fff-110">Attributes</span></span>

<span data-ttu-id="76fff-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="76fff-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76fff-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="76fff-112">Child elements</span></span>

|<span data-ttu-id="76fff-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="76fff-113">**Element**</span></span>|<span data-ttu-id="76fff-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="76fff-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76fff-115">FolderChange</span><span class="sxs-lookup"><span data-stu-id="76fff-115">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="76fff-116">Représente une modification unique à effectuer sur un seul dossier.</span><span class="sxs-lookup"><span data-stu-id="76fff-116">Represents a single change to be performed on a single folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76fff-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="76fff-117">Parent elements</span></span>

|<span data-ttu-id="76fff-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="76fff-118">**Element**</span></span>|<span data-ttu-id="76fff-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="76fff-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76fff-120">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="76fff-120">UpdateFolder</span></span>](updatefolder.md) <br/> |<span data-ttu-id="76fff-121">Représente l’opération utilisée pour mettre à jour les propriétés d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="76fff-121">Represents the operation that is used to update properties for a folder.</span></span>  <br/> <span data-ttu-id="76fff-122">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="76fff-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="76fff-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="76fff-123">Remarks</span></span>

<span data-ttu-id="76fff-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="76fff-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76fff-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="76fff-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76fff-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="76fff-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="76fff-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="76fff-127">Schema Name</span></span>  <br/> |<span data-ttu-id="76fff-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="76fff-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="76fff-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="76fff-129">Validation File</span></span>  <br/> |<span data-ttu-id="76fff-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="76fff-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76fff-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="76fff-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="76fff-132">False</span><span class="sxs-lookup"><span data-stu-id="76fff-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76fff-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="76fff-133">See also</span></span>



[<span data-ttu-id="76fff-134">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="76fff-134">UpdateFolder operation</span></span>](updatefolder-operation.md)

