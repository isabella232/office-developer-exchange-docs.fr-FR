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
description: L’élément CreateFolder définit une demande de création d’un dossier dans la Banque d’Exchange.
ms.openlocfilehash: c2a971a6b827553a1632c2a86e4d36e3b83a2de3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457542"
---
# <a name="createfolder"></a><span data-ttu-id="8710d-103">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="8710d-103">CreateFolder</span></span>

<span data-ttu-id="8710d-104">L’élément **CreateFolder** définit une demande de création d’un dossier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="8710d-104">The **CreateFolder** element defines a request to create a folder in the Exchange store.</span></span> 
  
```xml
<CreateFolder>
   <ParentFolderId/>
   <Folders/>
</CreateFolder>
```

 <span data-ttu-id="8710d-105">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="8710d-105">**CreateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8710d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8710d-106">Attributes and elements</span></span>

<span data-ttu-id="8710d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8710d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8710d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8710d-108">Attributes</span></span>

<span data-ttu-id="8710d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8710d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8710d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8710d-110">Child elements</span></span>

|<span data-ttu-id="8710d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8710d-111">**Element**</span></span>|<span data-ttu-id="8710d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8710d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8710d-113">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="8710d-113">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="8710d-114">Élément qui identifie l’emplacement où le nouveau dossier est créé.</span><span class="sxs-lookup"><span data-stu-id="8710d-114">The element that identifies the location where the new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="8710d-115">Dossiers</span><span class="sxs-lookup"><span data-stu-id="8710d-115">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8710d-116">Élément qui contient tous les dossiers à créer.</span><span class="sxs-lookup"><span data-stu-id="8710d-116">The element that contains all the folders to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8710d-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8710d-117">Parent elements</span></span>

<span data-ttu-id="8710d-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8710d-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8710d-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="8710d-119">Remarks</span></span>

<span data-ttu-id="8710d-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8710d-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8710d-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8710d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8710d-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8710d-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8710d-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8710d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="8710d-124">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="8710d-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="8710d-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8710d-125">Validation File</span></span>  <br/> |<span data-ttu-id="8710d-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8710d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8710d-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8710d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="8710d-128">False</span><span class="sxs-lookup"><span data-stu-id="8710d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8710d-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8710d-129">See also</span></span>



[<span data-ttu-id="8710d-130">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="8710d-130">CreateFolder operation</span></span>](createfolder-operation.md)


[<span data-ttu-id="8710d-131">Création de dossiers (services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="8710d-131">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

