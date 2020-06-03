---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: L’élément SharedFolderId représente l’identificateur du dossier partagé dont l’identificateur de dossier local doit être renvoyé par une demande d’opération GetSharingFolder.
ms.openlocfilehash: 546e148540708725bcf335f39bf69d193124d210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466121"
---
# <a name="sharedfolderid"></a><span data-ttu-id="a0e4a-103">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="a0e4a-103">SharedFolderId</span></span>

<span data-ttu-id="a0e4a-104">L’élément **SharedFolderId** représente l’identificateur du dossier partagé dont l’identificateur de dossier local doit être renvoyé par une demande d' [opération GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a0e4a-104">The **SharedFolderId** element represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<SharedFolderId/>
```

 <span data-ttu-id="a0e4a-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="a0e4a-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0e4a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a0e4a-106">Attributes and elements</span></span>

<span data-ttu-id="a0e4a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a0e4a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0e4a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a0e4a-108">Attributes</span></span>

<span data-ttu-id="a0e4a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a0e4a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0e4a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a0e4a-110">Child elements</span></span>

<span data-ttu-id="a0e4a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a0e4a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0e4a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a0e4a-112">Parent elements</span></span>

|<span data-ttu-id="a0e4a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0e4a-113">**Element**</span></span>|<span data-ttu-id="a0e4a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0e4a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0e4a-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="a0e4a-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="a0e4a-116">Définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié.</span><span class="sxs-lookup"><span data-stu-id="a0e4a-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a0e4a-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a0e4a-117">Text value</span></span>

<span data-ttu-id="a0e4a-118">La valeur de texte est une chaîne qui représente l’identificateur du dossier partagé dont l’identificateur de dossier local doit être renvoyé par une demande d' [opération GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a0e4a-118">The text value is a string that represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a0e4a-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="a0e4a-119">Remarks</span></span>

<span data-ttu-id="a0e4a-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0e4a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0e4a-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a0e4a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0e4a-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a0e4a-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a0e4a-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a0e4a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="a0e4a-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a0e4a-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a0e4a-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a0e4a-125">Validation File</span></span>  <br/> |<span data-ttu-id="a0e4a-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a0e4a-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0e4a-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a0e4a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0e4a-128">False</span><span class="sxs-lookup"><span data-stu-id="a0e4a-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0e4a-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a0e4a-129">See also</span></span>



[<span data-ttu-id="a0e4a-130">Opération GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="a0e4a-130">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="a0e4a-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a0e4a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

