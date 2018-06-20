---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: L’élément ParentFolderId identifie le dossier dans lequel un nouveau dossier est créé ou du dossier de recherche pour l’opération FindConversation.
ms.openlocfilehash: 61072e1dd3321beb5f3b76d9accf20530b443796
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828686"
---
# <a name="parentfolderid-targetfolderidtype"></a><span data-ttu-id="6fdaf-103">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="6fdaf-103">ParentFolderId (TargetFolderIdType)</span></span>

<span data-ttu-id="6fdaf-104">L’élément **ParentFolderId** identifie le dossier dans lequel un nouveau dossier est créé ou du dossier de recherche pour l' [opération FindConversation](findconversation-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6fdaf-104">The **ParentFolderId** element identifies the folder in which a new folder is created or the folder to search for the [FindConversation operation](findconversation-operation.md).</span></span>
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

<span data-ttu-id="6fdaf-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="6fdaf-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6fdaf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6fdaf-106">Attributes and elements</span></span>

<span data-ttu-id="6fdaf-107">L’élément **ParentFolderId** contient deux éléments enfants.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-107">The **ParentFolderId** element contains two child elements.</span></span> <span data-ttu-id="6fdaf-108">Les éléments enfants s’excluent mutuellement dans le schéma.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-108">The child elements are mutually exclusive in the schema.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="6fdaf-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="6fdaf-109">Attributes</span></span>

<span data-ttu-id="6fdaf-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6fdaf-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6fdaf-111">Child elements</span></span>

|<span data-ttu-id="6fdaf-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6fdaf-112">**Element**</span></span>|<span data-ttu-id="6fdaf-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="6fdaf-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fdaf-114">FolderId</span><span class="sxs-lookup"><span data-stu-id="6fdaf-114">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="6fdaf-115">Contient l’identificateur et la clé de changement facultatif d’un dossier dans lequel un nouveau dossier est créé ou le dossier est recherché dans l' [opération FindConversation](findconversation-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6fdaf-115">Contains the required identifier and the optional change key of a folder in which a new folder is created or the folder that is searched for the [FindConversation operation](findconversation-operation.md).</span></span> <span data-ttu-id="6fdaf-116">À l’aide de cet élément exclut l’utilisation de l’élément [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="6fdaf-116">Using this element excludes the use of the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="6fdaf-117">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="6fdaf-117">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="6fdaf-118">Identifie les dossiers de Microsoft Exchange Server 2007 par défaut.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-118">Identifies default Microsoft Exchange Server 2007 folders.</span></span> <span data-ttu-id="6fdaf-119">À l’aide de cet élément exclut l’utilisation de l’élément [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="6fdaf-119">Using this element excludes the use of the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6fdaf-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6fdaf-120">Parent elements</span></span>

|<span data-ttu-id="6fdaf-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6fdaf-121">**Element**</span></span>|<span data-ttu-id="6fdaf-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="6fdaf-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fdaf-123">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="6fdaf-123">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="6fdaf-124">Définit une demande pour créer un dossier dans la base de données Exchange.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-124">Defines a request to create a folder in the Exchange database.</span></span>  <br/> <span data-ttu-id="6fdaf-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/CreateFolder`</span><span class="sxs-lookup"><span data-stu-id="6fdaf-125">The following is the XPath expression to this element:  `/CreateFolder`</span></span> <br/> |
|[<span data-ttu-id="6fdaf-126">FindConversation</span><span class="sxs-lookup"><span data-stu-id="6fdaf-126">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="6fdaf-127">Définit une requête pour rechercher les conversations dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-127">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6fdaf-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6fdaf-128">Text value</span></span>

<span data-ttu-id="6fdaf-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6fdaf-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="6fdaf-130">Remarks</span></span>

<span data-ttu-id="6fdaf-131">Les deux éléments enfants sont utilisés pour définir le dossier qui contiendra le nouveau dossier.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-131">The two child elements are used to define the folder that will contain the new folder.</span></span> <span data-ttu-id="6fdaf-132">Vous devez sélectionner le [FolderId](folderid.md) ou l’élément [DistinguishedFolderId](distinguishedfolderid.md) pour identifier le dossier parent du nouveau dossier.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-132">You must select either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element to identify the parent folder of the new folder.</span></span> <span data-ttu-id="6fdaf-133">Vous ne pouvez pas utiliser les deux éléments en même temps.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-133">You cannot use both elements at the same time.</span></span> <span data-ttu-id="6fdaf-134">Cet élément est nécessaire pour créer des dossiers.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-134">This element is required to create folders.</span></span> 
  
<span data-ttu-id="6fdaf-135">L’élément [ParentFolderId](parentfolderid.md) décrit l’emplacement des éléments et dossiers existants.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-135">The [ParentFolderId](parentfolderid.md) element describes the location of existing items and folders.</span></span> 
  
<span data-ttu-id="6fdaf-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6fdaf-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6fdaf-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6fdaf-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6fdaf-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6fdaf-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6fdaf-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6fdaf-139">Schema Name</span></span>  <br/> |<span data-ttu-id="6fdaf-140">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="6fdaf-140">Message schema</span></span>  <br/> |
|<span data-ttu-id="6fdaf-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6fdaf-141">Validation File</span></span>  <br/> |<span data-ttu-id="6fdaf-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6fdaf-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6fdaf-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6fdaf-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="6fdaf-144">False</span><span class="sxs-lookup"><span data-stu-id="6fdaf-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6fdaf-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6fdaf-145">See also</span></span>

- [<span data-ttu-id="6fdaf-146">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="6fdaf-146">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="6fdaf-147">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="6fdaf-147">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="6fdaf-148">Création de dossiers (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="6fdaf-148">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

