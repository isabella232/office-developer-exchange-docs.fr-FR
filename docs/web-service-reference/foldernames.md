---
title: Noms de dossier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderNames
api_type:
- schema
ms.assetid: 6cbe4083-5705-4695-a54e-8dab3e472662
description: L’élément de noms de dossier contient un tableau des dossiers gérés nommées à ajouter à une boîte aux lettres.
ms.openlocfilehash: 819b3c2df1cfcae3a5d4a48539e369a00b1f7229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756452"
---
# <a name="foldernames"></a><span data-ttu-id="22c96-103">Noms de dossier</span><span class="sxs-lookup"><span data-stu-id="22c96-103">FolderNames</span></span>

<span data-ttu-id="22c96-104">L’élément de **noms de dossier** contient un tableau des dossiers gérés nommées à ajouter à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="22c96-104">The **FolderNames** element contains an array of named managed folders to add to a mailbox.</span></span> 
  
[<span data-ttu-id="22c96-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="22c96-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="22c96-106">Noms de dossier</span><span class="sxs-lookup"><span data-stu-id="22c96-106">FolderNames</span></span>](foldernames.md)
  
```xml
<FolderNames>
   <FolderName/>
</FolderNames>
```

 <span data-ttu-id="22c96-107">**NonEmptyArrayOfFolderNamesType**</span><span class="sxs-lookup"><span data-stu-id="22c96-107">**NonEmptyArrayOfFolderNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22c96-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22c96-108">Attributes and elements</span></span>

<span data-ttu-id="22c96-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22c96-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22c96-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="22c96-110">Attributes</span></span>

<span data-ttu-id="22c96-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="22c96-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22c96-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22c96-112">Child elements</span></span>

|<span data-ttu-id="22c96-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22c96-113">**Element**</span></span>|<span data-ttu-id="22c96-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="22c96-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22c96-115">FolderName</span><span class="sxs-lookup"><span data-stu-id="22c96-115">FolderName</span></span>](foldername.md) <br/> |<span data-ttu-id="22c96-116">Identifie un dossier géré unique à ajouter à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="22c96-116">Identifies a single managed folder to add to mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22c96-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22c96-117">Parent elements</span></span>

|<span data-ttu-id="22c96-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22c96-118">**Element**</span></span>|<span data-ttu-id="22c96-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="22c96-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22c96-120">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="22c96-120">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="22c96-121">L’élément racine dans une demande pour ajouter un dossier géré à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="22c96-121">The root element in a request to add a managed folder to a mailbox.</span></span>  <br/> <span data-ttu-id="22c96-122">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="22c96-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="22c96-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="22c96-123">Remarks</span></span>

<span data-ttu-id="22c96-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="22c96-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22c96-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22c96-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22c96-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22c96-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="22c96-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22c96-127">Schema Name</span></span>  <br/> |<span data-ttu-id="22c96-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="22c96-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="22c96-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22c96-129">Validation File</span></span>  <br/> |<span data-ttu-id="22c96-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="22c96-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="22c96-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22c96-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="22c96-132">False</span><span class="sxs-lookup"><span data-stu-id="22c96-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22c96-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22c96-133">See also</span></span>



[<span data-ttu-id="22c96-134">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="22c96-134">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="22c96-135">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="22c96-135">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="22c96-136">Ajout de dossiers gérés</span><span class="sxs-lookup"><span data-stu-id="22c96-136">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

