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
ms.openlocfilehash: e0eb1fbd7155040508daf253f5eb4b1352d7426d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829485"
---
# <a name="sharingfolderid"></a><span data-ttu-id="d3747-103">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="d3747-103">SharingFolderId</span></span>

<span data-ttu-id="d3747-104">L’élément **SharingFolderId** représente l’identificateur du dossier local dans une relation de partage.</span><span class="sxs-lookup"><span data-stu-id="d3747-104">The **SharingFolderId** element represents the identifier of the local folder in a sharing relationship.</span></span> 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="d3747-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="d3747-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3747-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d3747-106">Attributes and elements</span></span>

<span data-ttu-id="d3747-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d3747-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3747-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d3747-108">Attributes</span></span>

|<span data-ttu-id="d3747-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d3747-109">**Attribute**</span></span>|<span data-ttu-id="d3747-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3747-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d3747-111">ID</span><span class="sxs-lookup"><span data-stu-id="d3747-111">Id</span></span>  <br/> |<span data-ttu-id="d3747-112">Contient une chaîne qui identifie un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3747-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="d3747-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="d3747-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d3747-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="d3747-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="d3747-115">Contient une chaîne qui identifie une version d’un dossier qui est identifié par l’attribut Id.</span><span class="sxs-lookup"><span data-stu-id="d3747-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="d3747-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d3747-116">This attribute is optional.</span></span> <span data-ttu-id="d3747-117">Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.</span><span class="sxs-lookup"><span data-stu-id="d3747-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d3747-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d3747-118">Child elements</span></span>

<span data-ttu-id="d3747-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d3747-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d3747-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d3747-120">Parent elements</span></span>

|<span data-ttu-id="d3747-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3747-121">**Element**</span></span>|<span data-ttu-id="d3747-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3747-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3747-123">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="d3747-123">RefreshSharingFolder</span></span>](refreshsharingfolder.md) <br/> |<span data-ttu-id="d3747-124">Définit une demande pour actualiser le dossier local spécifié.</span><span class="sxs-lookup"><span data-stu-id="d3747-124">Defines a request to refresh the specified local folder.</span></span>  <br/> |
|[<span data-ttu-id="d3747-125">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="d3747-125">GetSharingFolderResponse</span></span>](getsharingfolderresponse.md) <br/> |<span data-ttu-id="d3747-126">Définit une réponse à une demande [d’opération GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d3747-126">Defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="d3747-127">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d3747-127">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="d3747-128">Contient l’état et les résultats d’une seule demande [d’opération GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d3747-128">Contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3747-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="d3747-129">Remarks</span></span>

<span data-ttu-id="d3747-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="d3747-130">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3747-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d3747-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3747-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d3747-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d3747-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d3747-133">Schema Name</span></span>  <br/> |<span data-ttu-id="d3747-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d3747-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d3747-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d3747-135">Validation File</span></span>  <br/> |<span data-ttu-id="d3747-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d3747-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d3747-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d3747-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3747-138">False</span><span class="sxs-lookup"><span data-stu-id="d3747-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3747-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d3747-139">See also</span></span>



- [<span data-ttu-id="d3747-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d3747-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

