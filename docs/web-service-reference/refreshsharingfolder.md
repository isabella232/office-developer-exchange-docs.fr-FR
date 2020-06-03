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
description: L’élément RefreshSharingFolder définit une demande d’actualisation du dossier local spécifié. Il s’agit de l’élément de base pour l’opération RefreshSharingFolder.
ms.openlocfilehash: 4454607fa2c3114cc7279fd7c30f8aee74707baa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467927"
---
# <a name="refreshsharingfolder"></a><span data-ttu-id="ba9da-104">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="ba9da-104">RefreshSharingFolder</span></span>

<span data-ttu-id="ba9da-105">L’élément **RefreshSharingFolder** définit une demande d’actualisation du dossier local spécifié.</span><span class="sxs-lookup"><span data-stu-id="ba9da-105">The **RefreshSharingFolder** element defines a request to refresh the specified local folder.</span></span> <span data-ttu-id="ba9da-106">Il s’agit de l’élément de base pour l' [opération RefreshSharingFolder](refreshsharingfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ba9da-106">It is the base element for the [RefreshSharingFolder operation](refreshsharingfolder-operation.md).</span></span>
  
```xml
<RefreshSharingFolder>   <SharingFolderId/></RefreshSharingFolder>
```

 <span data-ttu-id="ba9da-107">**RefreshSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="ba9da-107">**RefreshSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba9da-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ba9da-108">Attributes and elements</span></span>

<span data-ttu-id="ba9da-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ba9da-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba9da-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ba9da-110">Attributes</span></span>

<span data-ttu-id="ba9da-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ba9da-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba9da-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ba9da-112">Child elements</span></span>

|<span data-ttu-id="ba9da-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ba9da-113">**Element**</span></span>|<span data-ttu-id="ba9da-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba9da-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba9da-115">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="ba9da-115">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="ba9da-116">Représente l’identificateur du dossier local dans une relation de partage.</span><span class="sxs-lookup"><span data-stu-id="ba9da-116">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ba9da-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ba9da-117">Parent elements</span></span>

<span data-ttu-id="ba9da-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba9da-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ba9da-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="ba9da-119">Remarks</span></span>

<span data-ttu-id="ba9da-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ba9da-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba9da-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ba9da-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba9da-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ba9da-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ba9da-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ba9da-123">Schema Name</span></span>  <br/> |<span data-ttu-id="ba9da-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ba9da-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ba9da-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ba9da-125">Validation File</span></span>  <br/> |<span data-ttu-id="ba9da-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ba9da-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ba9da-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ba9da-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba9da-128">False</span><span class="sxs-lookup"><span data-stu-id="ba9da-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba9da-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ba9da-129">See also</span></span>



- [<span data-ttu-id="ba9da-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba9da-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

