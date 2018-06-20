---
title: SetTelephoneAccessFolderEmail (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 90759da7-6dba-499e-b8c8-e44a016b3198
description: L’élément SetTelephoneAccessFolderEmail définit une demande pour définir le dossier par défaut des messages électroniques à partir de laquelle la messagerie unifiée sera lire des messages par téléphone.
ms.openlocfilehash: e19f151e364411717d5129cbef8c5cc097689f89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829461"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a><span data-ttu-id="c4e21-103">SetTelephoneAccessFolderEmail (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="c4e21-103">SetTelephoneAccessFolderEmail (UM web service)</span></span>

<span data-ttu-id="c4e21-104">L’élément **SetTelephoneAccessFolderEmail** définit une demande pour définir le dossier par défaut des messages électroniques à partir de laquelle la messagerie unifiée sera lire des messages par téléphone.</span><span class="sxs-lookup"><span data-stu-id="c4e21-104">The **SetTelephoneAccessFolderEmail** element defines a request to set the default e-mail folder from which Unified Messaging will read messages over the telephone.</span></span> 
  
[<span data-ttu-id="c4e21-105">SetTelephoneAccessFolderEmail (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="c4e21-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 <span data-ttu-id="c4e21-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="c4e21-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4e21-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c4e21-107">Attributes and elements</span></span>

<span data-ttu-id="c4e21-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c4e21-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4e21-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="c4e21-109">Attributes</span></span>

<span data-ttu-id="c4e21-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c4e21-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4e21-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c4e21-111">Child elements</span></span>

|<span data-ttu-id="c4e21-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c4e21-112">**Element**</span></span>|<span data-ttu-id="c4e21-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="c4e21-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4e21-114">base64FolderId (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="c4e21-114">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md) <br/> |<span data-ttu-id="c4e21-115">L’identificateur du dossier de courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="c4e21-115">The identifier of the e-mail folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c4e21-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c4e21-116">Parent elements</span></span>

<span data-ttu-id="c4e21-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c4e21-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c4e21-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c4e21-118">Text value</span></span>

<span data-ttu-id="c4e21-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c4e21-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4e21-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c4e21-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4e21-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c4e21-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c4e21-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c4e21-122">Schema Name</span></span>  <br/> |<span data-ttu-id="c4e21-123">Messages</span><span class="sxs-lookup"><span data-stu-id="c4e21-123">Messages</span></span>  <br/> |
|<span data-ttu-id="c4e21-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c4e21-124">Validation File</span></span>  <br/> |<span data-ttu-id="c4e21-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c4e21-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c4e21-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c4e21-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="c4e21-127">False</span><span class="sxs-lookup"><span data-stu-id="c4e21-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4e21-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c4e21-128">See also</span></span>



[<span data-ttu-id="c4e21-129">Opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="c4e21-129">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)

