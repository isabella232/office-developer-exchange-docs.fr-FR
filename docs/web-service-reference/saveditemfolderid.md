---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: L’élément SavedItemFolderId identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans une boîte aux lettres.
ms.openlocfilehash: c57a7fb4abc2f7ee7b599f56f016811d6ff2c21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829277"
---
# <a name="saveditemfolderid"></a><span data-ttu-id="8e16e-103">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="8e16e-103">SavedItemFolderId</span></span>

<span data-ttu-id="8e16e-104">L’élément **SavedItemFolderId** identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8e16e-104">The **SavedItemFolderId** element identifies the target folder for operations that update, send, and create items in a mailbox.</span></span> 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

 <span data-ttu-id="8e16e-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="8e16e-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e16e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8e16e-106">Attributes and elements</span></span>

<span data-ttu-id="8e16e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8e16e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e16e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8e16e-108">Attributes</span></span>

<span data-ttu-id="8e16e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8e16e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e16e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8e16e-110">Child elements</span></span>

|<span data-ttu-id="8e16e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8e16e-111">**Element**</span></span>|<span data-ttu-id="8e16e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8e16e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e16e-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="8e16e-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="8e16e-114">Contient la clé d’identificateur et de modification d’un dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e16e-114">Contains the identifier and change key of a target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8e16e-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="8e16e-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="8e16e-116">Identifie un dossier cible par un identificateur nommé pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e16e-116">Identifies a target folder by a named identifier for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8e16e-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8e16e-117">Parent elements</span></span>

|<span data-ttu-id="8e16e-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8e16e-118">**Element**</span></span>|<span data-ttu-id="8e16e-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="8e16e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e16e-120">CreateItem</span><span class="sxs-lookup"><span data-stu-id="8e16e-120">CreateItem</span></span>](createitem.md) <br/> |<span data-ttu-id="8e16e-121">Définit une demande pour créer un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e16e-121">Defines a request to create an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="8e16e-122">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="8e16e-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateItem` <br/> |
|[<span data-ttu-id="8e16e-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="8e16e-123">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="8e16e-124">Définit une demande de mise à jour d’un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e16e-124">Defines a request to update an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="8e16e-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="8e16e-125">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
|[<span data-ttu-id="8e16e-126">SendItem</span><span class="sxs-lookup"><span data-stu-id="8e16e-126">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="8e16e-127">Définit une demande d’envoi d’un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e16e-127">Defines a request to send an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="8e16e-128">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="8e16e-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8e16e-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="8e16e-129">Remarks</span></span>

<span data-ttu-id="8e16e-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8e16e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e16e-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8e16e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e16e-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8e16e-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8e16e-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8e16e-133">Schema Name</span></span>  <br/> |<span data-ttu-id="8e16e-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8e16e-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8e16e-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8e16e-135">Validation File</span></span>  <br/> |<span data-ttu-id="8e16e-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8e16e-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8e16e-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8e16e-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e16e-138">False</span><span class="sxs-lookup"><span data-stu-id="8e16e-138">False</span></span>  <br/> |
   

