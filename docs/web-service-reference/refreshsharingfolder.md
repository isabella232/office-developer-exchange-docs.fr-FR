---
title: RefreshSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolder
api_type:
- schema
ms.assetid: 14571c28-effa-430a-802e-82fb99bafa7f
description: L’élément RefreshSharingFolder définit une demande pour actualiser le dossier local spécifié. Il s’agit de l’élément de base pour l’opération RefreshSharingFolder.
ms.openlocfilehash: b09e311d0ba38b0cdcc9fe0864ed3e2b0151b0fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829043"
---
# <a name="refreshsharingfolder"></a><span data-ttu-id="4c85a-104">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="4c85a-104">RefreshSharingFolder</span></span>

<span data-ttu-id="4c85a-105">L’élément **RefreshSharingFolder** définit une demande pour actualiser le dossier local spécifié.</span><span class="sxs-lookup"><span data-stu-id="4c85a-105">The **RefreshSharingFolder** element defines a request to refresh the specified local folder.</span></span> <span data-ttu-id="4c85a-106">Il s’agit de l’élément de base pour l' [opération RefreshSharingFolder](refreshsharingfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4c85a-106">It is the base element for the [RefreshSharingFolder operation](refreshsharingfolder-operation.md).</span></span>
  
```xml
<RefreshSharingFolder>   <SharingFolderId/></RefreshSharingFolder>
```

 <span data-ttu-id="4c85a-107">**RefreshSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="4c85a-107">**RefreshSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c85a-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4c85a-108">Attributes and elements</span></span>

<span data-ttu-id="4c85a-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4c85a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c85a-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="4c85a-110">Attributes</span></span>

<span data-ttu-id="4c85a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4c85a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c85a-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4c85a-112">Child elements</span></span>

|<span data-ttu-id="4c85a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4c85a-113">**Element**</span></span>|<span data-ttu-id="4c85a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="4c85a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c85a-115">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="4c85a-115">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="4c85a-116">Représente l’identificateur du dossier local dans une relation de partage.</span><span class="sxs-lookup"><span data-stu-id="4c85a-116">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4c85a-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4c85a-117">Parent elements</span></span>

<span data-ttu-id="4c85a-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4c85a-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4c85a-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="4c85a-119">Remarks</span></span>

<span data-ttu-id="4c85a-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="4c85a-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c85a-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4c85a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c85a-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4c85a-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4c85a-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4c85a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="4c85a-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4c85a-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4c85a-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4c85a-125">Validation File</span></span>  <br/> |<span data-ttu-id="4c85a-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4c85a-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4c85a-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4c85a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="4c85a-128">False</span><span class="sxs-lookup"><span data-stu-id="4c85a-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4c85a-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4c85a-129">See also</span></span>



- [<span data-ttu-id="4c85a-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4c85a-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

