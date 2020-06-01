---
title: SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)
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
description: L’élément SetTelephoneAccessFolderEmail définit une demande de définition du dossier de messagerie électronique par défaut à partir duquel la messagerie unifiée lira les messages par téléphone.
ms.openlocfilehash: 806bdb1f0c7930a9e89555192aa32ad997716e7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467318"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a><span data-ttu-id="c99ac-103">SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="c99ac-103">SetTelephoneAccessFolderEmail (UM web service)</span></span>

<span data-ttu-id="c99ac-104">L’élément **SetTelephoneAccessFolderEmail** définit une demande de définition du dossier de messagerie électronique par défaut à partir duquel la messagerie unifiée lira les messages par téléphone.</span><span class="sxs-lookup"><span data-stu-id="c99ac-104">The **SetTelephoneAccessFolderEmail** element defines a request to set the default e-mail folder from which Unified Messaging will read messages over the telephone.</span></span> 
  
[<span data-ttu-id="c99ac-105">SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="c99ac-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 <span data-ttu-id="c99ac-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="c99ac-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c99ac-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c99ac-107">Attributes and elements</span></span>

<span data-ttu-id="c99ac-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c99ac-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c99ac-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="c99ac-109">Attributes</span></span>

<span data-ttu-id="c99ac-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c99ac-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c99ac-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c99ac-111">Child elements</span></span>

|<span data-ttu-id="c99ac-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c99ac-112">**Element**</span></span>|<span data-ttu-id="c99ac-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="c99ac-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c99ac-114">base64FolderId (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="c99ac-114">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md) <br/> |<span data-ttu-id="c99ac-115">Identificateur du dossier de messagerie.</span><span class="sxs-lookup"><span data-stu-id="c99ac-115">The identifier of the e-mail folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c99ac-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c99ac-116">Parent elements</span></span>

<span data-ttu-id="c99ac-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c99ac-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c99ac-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c99ac-118">Text value</span></span>

<span data-ttu-id="c99ac-119">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c99ac-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c99ac-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c99ac-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c99ac-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c99ac-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c99ac-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c99ac-122">Schema Name</span></span>  <br/> |<span data-ttu-id="c99ac-123">Messages</span><span class="sxs-lookup"><span data-stu-id="c99ac-123">Messages</span></span>  <br/> |
|<span data-ttu-id="c99ac-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c99ac-124">Validation File</span></span>  <br/> |<span data-ttu-id="c99ac-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c99ac-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c99ac-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c99ac-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="c99ac-127">False</span><span class="sxs-lookup"><span data-stu-id="c99ac-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c99ac-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c99ac-128">See also</span></span>



[<span data-ttu-id="c99ac-129">Opération SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="c99ac-129">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)

