---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: L’élément NomDossier identifie un dossier personnalisé géré unique à ajouter à une boîte aux lettres.
ms.openlocfilehash: 1bb63e50c06e81337d1142a6624213fb2db12457
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461351"
---
# <a name="foldername"></a><span data-ttu-id="5e55c-103">FolderName</span><span class="sxs-lookup"><span data-stu-id="5e55c-103">FolderName</span></span>

<span data-ttu-id="5e55c-104">L’élément **NomDossier** identifie un dossier personnalisé géré unique à ajouter à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5e55c-104">The **FolderName** element identifies a single managed custom folder to add to a mailbox.</span></span> 
  
[<span data-ttu-id="5e55c-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="5e55c-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="5e55c-106">FolderNames</span><span class="sxs-lookup"><span data-stu-id="5e55c-106">FolderNames</span></span>](foldernames.md)
  
[<span data-ttu-id="5e55c-107">FolderName</span><span class="sxs-lookup"><span data-stu-id="5e55c-107">FolderName</span></span>](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 <span data-ttu-id="5e55c-108">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="5e55c-108">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e55c-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5e55c-109">Attributes and elements</span></span>

<span data-ttu-id="5e55c-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5e55c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e55c-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="5e55c-111">Attributes</span></span>

<span data-ttu-id="5e55c-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5e55c-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e55c-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5e55c-113">Child elements</span></span>

<span data-ttu-id="5e55c-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5e55c-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5e55c-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5e55c-115">Parent elements</span></span>

|<span data-ttu-id="5e55c-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5e55c-116">**Element**</span></span>|<span data-ttu-id="5e55c-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="5e55c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e55c-118">FolderNames</span><span class="sxs-lookup"><span data-stu-id="5e55c-118">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="5e55c-119">Contient un tableau de dossiers personnalisés gérés nommés à ajouter à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5e55c-119">Contains an array of named managed custom folders to add to a mailbox.</span></span>  <br/> <span data-ttu-id="5e55c-120">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="5e55c-120">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5e55c-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5e55c-121">Text value</span></span>

<span data-ttu-id="5e55c-122">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="5e55c-122">A text value is required.</span></span> <span data-ttu-id="5e55c-123">La valeur texte représente un nom de dossier.</span><span class="sxs-lookup"><span data-stu-id="5e55c-123">The text value represents a folder name.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5e55c-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="5e55c-124">Remarks</span></span>

<span data-ttu-id="5e55c-125">Bien que vous puissiez utiliser les services Web Exchange pour ajouter des dossiers personnalisés gérés à une boîte aux lettres, vous ne pouvez pas utiliser la même technologie pour accéder à la liste des dossiers personnalisés gérés disponibles.</span><span class="sxs-lookup"><span data-stu-id="5e55c-125">Although you can use Exchange Web Services to add managed custom folders to a mailbox, you cannot use the same technology to access the list of available managed custom folders.</span></span> <span data-ttu-id="5e55c-126">Vous pouvez obtenir la liste des dossiers personnalisés gérés à l’aide d’une commande de l’environnement de commande Exchange Management Shell ou à l’aide d’une API qui interface avec le service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5e55c-126">You can obtain a list of managed custom folders by using an Exchange Management Shell command or by using an API that interfaces with the Active Directory directory service.</span></span> <span data-ttu-id="5e55c-127">Le nom du dossier est le nom de l’objet Active Directory correspondant.</span><span class="sxs-lookup"><span data-stu-id="5e55c-127">The folder name is the name of the corresponding Active Directory object.</span></span>
  
<span data-ttu-id="5e55c-128">Vous pouvez utiliser l' [opération FindFolder](findfolder-operation.md) pour rechercher des dossiers personnalisés gérés.</span><span class="sxs-lookup"><span data-stu-id="5e55c-128">You can use the [FindFolder operation](findfolder-operation.md) to find managed custom folders.</span></span> <span data-ttu-id="5e55c-129">Utilisez l' [opération DeleteFolder](deletefolder-operation.md) pour supprimer des dossiers personnalisés gérés.</span><span class="sxs-lookup"><span data-stu-id="5e55c-129">Use the [DeleteFolder operation](deletefolder-operation.md) to delete managed custom folders.</span></span> 
  
<span data-ttu-id="5e55c-130">Il est important de noter que **NomDossier** est le nom d’un dossier personnalisé géré existant dans l’organisation.</span><span class="sxs-lookup"><span data-stu-id="5e55c-130">It is important to note that **FolderName** is the name of an existing managed custom folder in the organization.</span></span> <span data-ttu-id="5e55c-131">Une tentative d’ajout d’un dossier qui ne se trouve pas dans l’organisation entraîne une erreur de réponse.</span><span class="sxs-lookup"><span data-stu-id="5e55c-131">An attempt to add a folder that is not in the organization will result in an error response.</span></span> 
  
<span data-ttu-id="5e55c-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5e55c-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5e55c-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5e55c-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e55c-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5e55c-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5e55c-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5e55c-135">Schema Name</span></span>  <br/> |<span data-ttu-id="5e55c-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5e55c-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="5e55c-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5e55c-137">Validation File</span></span>  <br/> |<span data-ttu-id="5e55c-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5e55c-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5e55c-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5e55c-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e55c-140">False</span><span class="sxs-lookup"><span data-stu-id="5e55c-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e55c-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5e55c-141">See also</span></span>



[<span data-ttu-id="5e55c-142">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="5e55c-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="5e55c-143">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="5e55c-143">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="5e55c-144">Ajout de dossiers gérés</span><span class="sxs-lookup"><span data-stu-id="5e55c-144">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

