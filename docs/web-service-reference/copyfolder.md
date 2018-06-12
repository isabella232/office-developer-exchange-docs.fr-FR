---
title: CopyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: 7d5cd08a-fe81-4cb6-a5a0-6dec2d3c93d4
description: L’élément CopyFolder définit une demande pour copier les dossiers dans une boîte aux lettres dans la banque d’informations Exchange.
ms.openlocfilehash: 7bcfcc7f4212b3a3bd339fa5863df2990eb20d6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755664"
---
# <a name="copyfolder"></a><span data-ttu-id="b4442-103">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="b4442-103">CopyFolder</span></span>

<span data-ttu-id="b4442-104">L’élément **CopyFolder** définit une demande pour copier les dossiers dans une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4442-104">The **CopyFolder** element defines a request to copy folders in a mailbox in the Exchange store.</span></span> 
  
```xml
<CopyFolder>
   <ToFolderId/>
   <FolderIds/>
</CopyFolder>
```

 <span data-ttu-id="b4442-105">**CopyFolderType**</span><span class="sxs-lookup"><span data-stu-id="b4442-105">**CopyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4442-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b4442-106">Attributes and elements</span></span>

<span data-ttu-id="b4442-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b4442-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4442-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b4442-108">Attributes</span></span>

<span data-ttu-id="b4442-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b4442-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4442-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b4442-110">Child elements</span></span>

|<span data-ttu-id="b4442-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b4442-111">**Element**</span></span>|<span data-ttu-id="b4442-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b4442-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4442-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="b4442-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="b4442-114">Représente le dossier de destination pour un dossier copié.</span><span class="sxs-lookup"><span data-stu-id="b4442-114">Represents the destination folder for a copied folder.</span></span>  <br/> |
|[<span data-ttu-id="b4442-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="b4442-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="b4442-116">Contient un tableau de dossiers à copier dans le dossier identifié par l’élément [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="b4442-116">Contains an array of folders to copy to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b4442-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b4442-117">Parent elements</span></span>

<span data-ttu-id="b4442-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b4442-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b4442-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="b4442-119">Remarks</span></span>

<span data-ttu-id="b4442-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b4442-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4442-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b4442-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4442-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b4442-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b4442-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b4442-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b4442-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b4442-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b4442-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b4442-125">Validation File</span></span>  <br/> |<span data-ttu-id="b4442-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b4442-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b4442-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b4442-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b4442-128">False</span><span class="sxs-lookup"><span data-stu-id="b4442-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b4442-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b4442-129">See also</span></span>



[<span data-ttu-id="b4442-130">Opération CopyFolder</span><span class="sxs-lookup"><span data-stu-id="b4442-130">CopyFolder operation</span></span>](copyfolder-operation.md)

