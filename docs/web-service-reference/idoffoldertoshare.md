---
title: IdOfFolderToShare
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IdOfFolderToShare
api_type:
- schema
ms.assetid: 199d1839-f061-4070-a977-874b0c08e5be
description: L’élément IdOfFolderToShare représente l’identificateur du dossier sur le serveur qui est partagé.
ms.openlocfilehash: 1e3e53819f23bbc5753ac21b9e3ea6593ac4826c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827853"
---
# <a name="idoffoldertoshare"></a><span data-ttu-id="4b5b2-103">IdOfFolderToShare</span><span class="sxs-lookup"><span data-stu-id="4b5b2-103">IdOfFolderToShare</span></span>

<span data-ttu-id="4b5b2-104">L’élément **IdOfFolderToShare** représente l’identificateur du dossier sur le serveur qui est partagé.</span><span class="sxs-lookup"><span data-stu-id="4b5b2-104">The **IdOfFolderToShare** element represents the identifier of the folder on the server that will be shared.</span></span> 
  
```
<IdOfFolderToShare Id="" ChangeKey="" />
```

 <span data-ttu-id="4b5b2-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="4b5b2-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b5b2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4b5b2-106">Attributes and elements</span></span>

<span data-ttu-id="4b5b2-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4b5b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b5b2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4b5b2-108">Attributes</span></span>

|<span data-ttu-id="4b5b2-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4b5b2-109">**Attribute**</span></span>|<span data-ttu-id="4b5b2-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b5b2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4b5b2-111">ID</span><span class="sxs-lookup"><span data-stu-id="4b5b2-111">Id</span></span>  <br/> |<span data-ttu-id="4b5b2-112">Contient une chaîne qui identifie un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b5b2-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="4b5b2-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="4b5b2-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="4b5b2-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="4b5b2-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="4b5b2-115">Contient une chaîne qui identifie une version d’un dossier qui est identifié par l’attribut Id.</span><span class="sxs-lookup"><span data-stu-id="4b5b2-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="4b5b2-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="4b5b2-116">This attribute is optional.</span></span> <span data-ttu-id="4b5b2-117">Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.</span><span class="sxs-lookup"><span data-stu-id="4b5b2-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4b5b2-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4b5b2-118">Child elements</span></span>

<span data-ttu-id="4b5b2-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4b5b2-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4b5b2-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4b5b2-120">Parent elements</span></span>

|<span data-ttu-id="4b5b2-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b5b2-121">**Element**</span></span>|<span data-ttu-id="4b5b2-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b5b2-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b5b2-123">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="4b5b2-123">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="4b5b2-124">Définit une demande pour obtenir un jeton d’authentification opaque qui identifie l’invitation de partage.</span><span class="sxs-lookup"><span data-stu-id="4b5b2-124">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4b5b2-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="4b5b2-125">Remarks</span></span>

<span data-ttu-id="4b5b2-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="4b5b2-126">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b5b2-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4b5b2-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b5b2-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4b5b2-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4b5b2-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4b5b2-129">Schema Name</span></span>  <br/> |<span data-ttu-id="4b5b2-130">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4b5b2-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4b5b2-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4b5b2-131">Validation File</span></span>  <br/> |<span data-ttu-id="4b5b2-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4b5b2-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4b5b2-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4b5b2-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b5b2-134">False</span><span class="sxs-lookup"><span data-stu-id="4b5b2-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b5b2-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b5b2-135">See also</span></span>



[<span data-ttu-id="4b5b2-136">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="4b5b2-136">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="4b5b2-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b5b2-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

