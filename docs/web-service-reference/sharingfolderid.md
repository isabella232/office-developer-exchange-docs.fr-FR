---
title: SharingFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: L’élément SharingFolderId représente l’identificateur du dossier local dans une relation de partage.
ms.openlocfilehash: 02780251639ee651ca65d8eadded43260852aaf8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526577"
---
# <a name="sharingfolderid"></a><span data-ttu-id="1d249-103">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="1d249-103">SharingFolderId</span></span>

<span data-ttu-id="1d249-104">L’élément **SharingFolderId** représente l’identificateur du dossier local dans une relation de partage.</span><span class="sxs-lookup"><span data-stu-id="1d249-104">The **SharingFolderId** element represents the identifier of the local folder in a sharing relationship.</span></span> 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="1d249-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="1d249-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d249-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1d249-106">Attributes and elements</span></span>

<span data-ttu-id="1d249-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1d249-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d249-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1d249-108">Attributes</span></span>

|<span data-ttu-id="1d249-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1d249-109">**Attribute**</span></span>|<span data-ttu-id="1d249-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="1d249-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1d249-111">ID</span><span class="sxs-lookup"><span data-stu-id="1d249-111">Id</span></span>  <br/> |<span data-ttu-id="1d249-112">Contient une chaîne qui identifie un dossier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="1d249-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="1d249-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="1d249-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="1d249-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="1d249-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="1d249-115">Contient une chaîne qui identifie la version d’un dossier identifiée par l’attribut ID.</span><span class="sxs-lookup"><span data-stu-id="1d249-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="1d249-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="1d249-116">This attribute is optional.</span></span> <span data-ttu-id="1d249-117">Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.</span><span class="sxs-lookup"><span data-stu-id="1d249-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1d249-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1d249-118">Child elements</span></span>

<span data-ttu-id="1d249-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1d249-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1d249-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1d249-120">Parent elements</span></span>

|<span data-ttu-id="1d249-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1d249-121">**Element**</span></span>|<span data-ttu-id="1d249-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="1d249-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d249-123">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="1d249-123">RefreshSharingFolder</span></span>](refreshsharingfolder.md) <br/> |<span data-ttu-id="1d249-124">Définit une demande d’actualisation du dossier local spécifié.</span><span class="sxs-lookup"><span data-stu-id="1d249-124">Defines a request to refresh the specified local folder.</span></span>  <br/> |
|[<span data-ttu-id="1d249-125">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="1d249-125">GetSharingFolderResponse</span></span>](getsharingfolderresponse.md) <br/> |<span data-ttu-id="1d249-126">Définit une réponse à une demande d' [opération GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1d249-126">Defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="1d249-127">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1d249-127">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="1d249-128">Contient l’État et le résultat d’une seule demande d' [opération GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1d249-128">Contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1d249-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="1d249-129">Remarks</span></span>

<span data-ttu-id="1d249-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1d249-130">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d249-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1d249-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d249-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1d249-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1d249-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1d249-133">Schema Name</span></span>  <br/> |<span data-ttu-id="1d249-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1d249-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1d249-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1d249-135">Validation File</span></span>  <br/> |<span data-ttu-id="1d249-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1d249-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1d249-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1d249-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d249-138">False</span><span class="sxs-lookup"><span data-stu-id="1d249-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d249-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1d249-139">See also</span></span>



- [<span data-ttu-id="1d249-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1d249-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

