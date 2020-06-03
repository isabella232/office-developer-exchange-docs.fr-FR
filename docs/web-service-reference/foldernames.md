---
title: FolderNames
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
description: L’élément FolderNames contient un tableau de dossiers gérés nommés à ajouter à une boîte aux lettres.
ms.openlocfilehash: 00cb1a81f420469033ccbc745313d2719b155aff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530985"
---
# <a name="foldernames"></a><span data-ttu-id="e20ba-103">FolderNames</span><span class="sxs-lookup"><span data-stu-id="e20ba-103">FolderNames</span></span>

<span data-ttu-id="e20ba-104">L’élément **foldernames** contient un tableau de dossiers gérés nommés à ajouter à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e20ba-104">The **FolderNames** element contains an array of named managed folders to add to a mailbox.</span></span> 
  
[<span data-ttu-id="e20ba-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="e20ba-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="e20ba-106">FolderNames</span><span class="sxs-lookup"><span data-stu-id="e20ba-106">FolderNames</span></span>](foldernames.md)
  
```xml
<FolderNames>
   <FolderName/>
</FolderNames>
```

 <span data-ttu-id="e20ba-107">**NonEmptyArrayOfFolderNamesType**</span><span class="sxs-lookup"><span data-stu-id="e20ba-107">**NonEmptyArrayOfFolderNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e20ba-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e20ba-108">Attributes and elements</span></span>

<span data-ttu-id="e20ba-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e20ba-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e20ba-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="e20ba-110">Attributes</span></span>

<span data-ttu-id="e20ba-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e20ba-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e20ba-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e20ba-112">Child elements</span></span>

|<span data-ttu-id="e20ba-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e20ba-113">**Element**</span></span>|<span data-ttu-id="e20ba-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="e20ba-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e20ba-115">FolderName</span><span class="sxs-lookup"><span data-stu-id="e20ba-115">FolderName</span></span>](foldername.md) <br/> |<span data-ttu-id="e20ba-116">Identifie un dossier géré unique à ajouter à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e20ba-116">Identifies a single managed folder to add to mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e20ba-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e20ba-117">Parent elements</span></span>

|<span data-ttu-id="e20ba-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e20ba-118">**Element**</span></span>|<span data-ttu-id="e20ba-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="e20ba-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e20ba-120">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="e20ba-120">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="e20ba-121">Élément racine dans une demande d’ajout d’un dossier géré à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e20ba-121">The root element in a request to add a managed folder to a mailbox.</span></span>  <br/> <span data-ttu-id="e20ba-122">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="e20ba-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e20ba-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="e20ba-123">Remarks</span></span>

<span data-ttu-id="e20ba-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e20ba-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e20ba-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e20ba-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e20ba-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e20ba-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e20ba-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e20ba-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e20ba-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e20ba-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e20ba-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e20ba-129">Validation File</span></span>  <br/> |<span data-ttu-id="e20ba-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e20ba-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e20ba-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e20ba-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e20ba-132">False</span><span class="sxs-lookup"><span data-stu-id="e20ba-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e20ba-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e20ba-133">See also</span></span>



[<span data-ttu-id="e20ba-134">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="e20ba-134">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="e20ba-135">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="e20ba-135">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="e20ba-136">Ajout de dossiers gérés</span><span class="sxs-lookup"><span data-stu-id="e20ba-136">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

