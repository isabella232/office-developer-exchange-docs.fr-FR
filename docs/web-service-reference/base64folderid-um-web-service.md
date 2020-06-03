---
title: base64FolderId (service Web de messagerie unifiée)
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
description: L’élément base64FolderId contient l’identificateur du dossier à spécifier comme dossier de messagerie électronique par défaut à partir duquel la messagerie unifiée lit les messages sur le téléphone dans une demande SetTelephoneAccessFolderEmail Operation (service Web de messagerie unifiée).
ms.openlocfilehash: ea31c7a0f93188e563bf95c4a3e6e91f0866746c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458046"
---
# <a name="base64folderid-um-web-service"></a><span data-ttu-id="a404a-103">base64FolderId (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="a404a-103">base64FolderId (UM web service)</span></span>

<span data-ttu-id="a404a-104">L’élément **base64FolderId** contient l’identificateur du dossier à spécifier comme dossier de messagerie électronique par défaut à partir duquel la messagerie unifiée lit les messages sur le téléphone dans une demande [SetTelephoneAccessFolderEmail Operation (service Web de messagerie unifiée)](settelephoneaccessfolderemail-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="a404a-104">The **base64FolderId** element contains the identifier of the folder to specify as the default e-mail folder from which Unified Messaging reads messages over the telephone in a [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="a404a-105">SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="a404a-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="a404a-106">base64FolderId (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="a404a-106">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 <span data-ttu-id="a404a-107">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="a404a-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a404a-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a404a-108">Attributes and elements</span></span>

<span data-ttu-id="a404a-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a404a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a404a-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="a404a-110">Attributes</span></span>

<span data-ttu-id="a404a-111">Aucun</span><span class="sxs-lookup"><span data-stu-id="a404a-111">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a404a-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a404a-112">Child elements</span></span>

<span data-ttu-id="a404a-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a404a-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a404a-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a404a-114">Parent elements</span></span>

|<span data-ttu-id="a404a-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a404a-115">**Element**</span></span>|<span data-ttu-id="a404a-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="a404a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a404a-117">SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="a404a-117">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="a404a-118">Définit une demande de définition du dossier de messagerie d’accès téléphonique.</span><span class="sxs-lookup"><span data-stu-id="a404a-118">Defines request to set the telephone access e-mail folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a404a-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a404a-119">Text value</span></span>

<span data-ttu-id="a404a-120">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="a404a-120">A text value is required.</span></span> <span data-ttu-id="a404a-121">La valeur de texte représente l’ID MAPI du dossier.</span><span class="sxs-lookup"><span data-stu-id="a404a-121">The text value represents the MAPI ID of the folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a404a-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="a404a-122">Remarks</span></span>

<span data-ttu-id="a404a-123">Pour définir le dossier de messagerie d’accès téléphonique, utilisez l' [opération SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)](settelephoneaccessfolderemail-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="a404a-123">To set the telephone access e-mail folder, use the [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a404a-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a404a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a404a-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a404a-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a404a-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a404a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="a404a-127">Messages</span><span class="sxs-lookup"><span data-stu-id="a404a-127">Messages</span></span>  <br/> |
|<span data-ttu-id="a404a-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a404a-128">Validation File</span></span>  <br/> |<span data-ttu-id="a404a-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a404a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a404a-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a404a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="a404a-131">False</span><span class="sxs-lookup"><span data-stu-id="a404a-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a404a-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a404a-132">See also</span></span>



[<span data-ttu-id="a404a-133">SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="a404a-133">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="a404a-134">Opération SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="a404a-134">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[<span data-ttu-id="a404a-135">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="a404a-135">FindFolder operation</span></span>](findfolder-operation.md)
  
[<span data-ttu-id="a404a-136">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="a404a-136">FindItem operation</span></span>](finditem-operation.md)

