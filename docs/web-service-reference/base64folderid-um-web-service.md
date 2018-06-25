---
title: base64FolderId (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: L’élément base64FolderId contient l’identificateur du dossier pour spécifier que le dossier de courrier électronique par défaut à partir de laquelle la messagerie unifiée lit les messages par téléphone dans une requête (service web de messagerie unifiée) d’opération SetTelephoneAccessFolderEmail.
ms.openlocfilehash: 7d710542418a717c6fcad243a22682e5840ebbd2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755372"
---
# <a name="base64folderid-um-web-service"></a><span data-ttu-id="d1b59-103">base64FolderId (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d1b59-103">base64FolderId (UM web service)</span></span>

<span data-ttu-id="d1b59-104">L’élément **base64FolderId** contient l’identificateur du dossier pour spécifier que le dossier de courrier électronique par défaut à partir de laquelle la messagerie unifiée lit les messages par téléphone dans une requête [d’opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="d1b59-104">The **base64FolderId** element contains the identifier of the folder to specify as the default e-mail folder from which Unified Messaging reads messages over the telephone in a [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="d1b59-105">SetTelephoneAccessFolderEmail (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d1b59-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="d1b59-106">base64FolderId (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d1b59-106">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 <span data-ttu-id="d1b59-107">**string**</span><span class="sxs-lookup"><span data-stu-id="d1b59-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1b59-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d1b59-108">Attributes and elements</span></span>

<span data-ttu-id="d1b59-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d1b59-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1b59-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d1b59-110">Attributes</span></span>

<span data-ttu-id="d1b59-111">Aucun</span><span class="sxs-lookup"><span data-stu-id="d1b59-111">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1b59-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d1b59-112">Child elements</span></span>

<span data-ttu-id="d1b59-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d1b59-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1b59-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d1b59-114">Parent elements</span></span>

|<span data-ttu-id="d1b59-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d1b59-115">**Element**</span></span>|<span data-ttu-id="d1b59-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="d1b59-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1b59-117">SetTelephoneAccessFolderEmail (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d1b59-117">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="d1b59-118">Définit la demande pour définir le dossier de courrier électronique de l’accès téléphonique.</span><span class="sxs-lookup"><span data-stu-id="d1b59-118">Defines request to set the telephone access e-mail folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d1b59-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d1b59-119">Text value</span></span>

<span data-ttu-id="d1b59-120">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="d1b59-120">A text value is required.</span></span> <span data-ttu-id="d1b59-121">La valeur de text représente l’ID MAPI du dossier.</span><span class="sxs-lookup"><span data-stu-id="d1b59-121">The text value represents the MAPI ID of the folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d1b59-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="d1b59-122">Remarks</span></span>

<span data-ttu-id="d1b59-123">Pour définir le dossier de messages électroniques d’accès téléphonique, utilisez l' [opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="d1b59-123">To set the telephone access e-mail folder, use the [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1b59-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d1b59-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1b59-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d1b59-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d1b59-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d1b59-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d1b59-127">Messages</span><span class="sxs-lookup"><span data-stu-id="d1b59-127">Messages</span></span>  <br/> |
|<span data-ttu-id="d1b59-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d1b59-128">Validation File</span></span>  <br/> |<span data-ttu-id="d1b59-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d1b59-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d1b59-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d1b59-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1b59-131">False</span><span class="sxs-lookup"><span data-stu-id="d1b59-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1b59-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d1b59-132">See also</span></span>



[<span data-ttu-id="d1b59-133">SetTelephoneAccessFolderEmail (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d1b59-133">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="d1b59-134">Opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d1b59-134">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[<span data-ttu-id="d1b59-135">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="d1b59-135">FindFolder operation</span></span>](findfolder-operation.md)
  
[<span data-ttu-id="d1b59-136">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="d1b59-136">FindItem operation</span></span>](finditem-operation.md)

