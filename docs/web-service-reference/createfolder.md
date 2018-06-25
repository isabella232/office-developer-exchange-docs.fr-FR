---
title: CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 110bada1-517b-4bd6-870d-7086dc879e5d
description: L’élément CreateFolder définit une demande pour créer un dossier dans la banque d’informations Exchange.
ms.openlocfilehash: e30af23b8ed8669053b94be460d62fbf7abf24c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755695"
---
# <a name="createfolder"></a><span data-ttu-id="172a9-103">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="172a9-103">CreateFolder</span></span>

<span data-ttu-id="172a9-104">L’élément **CreateFolder** définit une demande pour créer un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="172a9-104">The **CreateFolder** element defines a request to create a folder in the Exchange store.</span></span> 
  
```xml
<CreateFolder>
   <ParentFolderId/>
   <Folders/>
</CreateFolder>
```

 <span data-ttu-id="172a9-105">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="172a9-105">**CreateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="172a9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="172a9-106">Attributes and elements</span></span>

<span data-ttu-id="172a9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="172a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="172a9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="172a9-108">Attributes</span></span>

<span data-ttu-id="172a9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="172a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="172a9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="172a9-110">Child elements</span></span>

|<span data-ttu-id="172a9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="172a9-111">**Element**</span></span>|<span data-ttu-id="172a9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="172a9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="172a9-113">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="172a9-113">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="172a9-114">L’élément qui identifie l’emplacement où le nouveau dossier est créé.</span><span class="sxs-lookup"><span data-stu-id="172a9-114">The element that identifies the location where the new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="172a9-115">Dossiers</span><span class="sxs-lookup"><span data-stu-id="172a9-115">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="172a9-116">L’élément qui contient tous les dossiers à créer.</span><span class="sxs-lookup"><span data-stu-id="172a9-116">The element that contains all the folders to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="172a9-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="172a9-117">Parent elements</span></span>

<span data-ttu-id="172a9-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="172a9-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="172a9-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="172a9-119">Remarks</span></span>

<span data-ttu-id="172a9-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="172a9-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="172a9-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="172a9-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="172a9-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="172a9-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="172a9-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="172a9-123">Schema Name</span></span>  <br/> |<span data-ttu-id="172a9-124">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="172a9-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="172a9-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="172a9-125">Validation File</span></span>  <br/> |<span data-ttu-id="172a9-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="172a9-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="172a9-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="172a9-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="172a9-128">False</span><span class="sxs-lookup"><span data-stu-id="172a9-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="172a9-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="172a9-129">See also</span></span>



[<span data-ttu-id="172a9-130">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="172a9-130">CreateFolder operation</span></span>](createfolder-operation.md)


[<span data-ttu-id="172a9-131">Création de dossiers (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="172a9-131">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

