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
description: L’élément CopyFolder définit une demande de copie des dossiers dans une boîte aux lettres dans la Banque d’Exchange.
ms.openlocfilehash: fa75272540169a96d5567181d27b8a8f056cce42
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452509"
---
# <a name="copyfolder"></a><span data-ttu-id="de3bd-103">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="de3bd-103">CopyFolder</span></span>

<span data-ttu-id="de3bd-104">L’élément **CopyFolder** définit une demande de copie des dossiers dans une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="de3bd-104">The **CopyFolder** element defines a request to copy folders in a mailbox in the Exchange store.</span></span> 
  
```xml
<CopyFolder>
   <ToFolderId/>
   <FolderIds/>
</CopyFolder>
```

 <span data-ttu-id="de3bd-105">**CopyFolderType**</span><span class="sxs-lookup"><span data-stu-id="de3bd-105">**CopyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de3bd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="de3bd-106">Attributes and elements</span></span>

<span data-ttu-id="de3bd-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="de3bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de3bd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="de3bd-108">Attributes</span></span>

<span data-ttu-id="de3bd-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="de3bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de3bd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="de3bd-110">Child elements</span></span>

|<span data-ttu-id="de3bd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="de3bd-111">**Element**</span></span>|<span data-ttu-id="de3bd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="de3bd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de3bd-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="de3bd-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="de3bd-114">Représente le dossier de destination d’un dossier copié.</span><span class="sxs-lookup"><span data-stu-id="de3bd-114">Represents the destination folder for a copied folder.</span></span>  <br/> |
|[<span data-ttu-id="de3bd-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="de3bd-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="de3bd-116">Contient un tableau de dossiers à copier dans le dossier identifié par l’élément [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="de3bd-116">Contains an array of folders to copy to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="de3bd-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="de3bd-117">Parent elements</span></span>

<span data-ttu-id="de3bd-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="de3bd-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="de3bd-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="de3bd-119">Remarks</span></span>

<span data-ttu-id="de3bd-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="de3bd-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de3bd-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="de3bd-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de3bd-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="de3bd-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="de3bd-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="de3bd-123">Schema Name</span></span>  <br/> |<span data-ttu-id="de3bd-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="de3bd-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="de3bd-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="de3bd-125">Validation File</span></span>  <br/> |<span data-ttu-id="de3bd-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="de3bd-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="de3bd-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="de3bd-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="de3bd-128">False</span><span class="sxs-lookup"><span data-stu-id="de3bd-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de3bd-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="de3bd-129">See also</span></span>



[<span data-ttu-id="de3bd-130">CopyFolder, opération</span><span class="sxs-lookup"><span data-stu-id="de3bd-130">CopyFolder operation</span></span>](copyfolder-operation.md)

