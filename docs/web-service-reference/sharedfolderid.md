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
description: L’élément SharedFolderId représente l’identificateur du dossier partagé pour lequel l’identificateur de dossier local doit être retournée par une requête d’opération GetSharingFolder.
ms.openlocfilehash: 6d4e541ef3cae89e413efa8cc5f1beaf651dc4dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829477"
---
# <a name="sharedfolderid"></a><span data-ttu-id="9fd2c-103">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="9fd2c-103">SharedFolderId</span></span>

<span data-ttu-id="9fd2c-104">L’élément **SharedFolderId** représente l’identificateur du dossier partagé pour lequel l’identificateur de dossier local doit être retournée par une demande [d’opération GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9fd2c-104">The **SharedFolderId** element represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<SharedFolderId/>
```

 <span data-ttu-id="9fd2c-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="9fd2c-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fd2c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9fd2c-106">Attributes and elements</span></span>

<span data-ttu-id="9fd2c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9fd2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fd2c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9fd2c-108">Attributes</span></span>

<span data-ttu-id="9fd2c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9fd2c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fd2c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9fd2c-110">Child elements</span></span>

<span data-ttu-id="9fd2c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9fd2c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9fd2c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9fd2c-112">Parent elements</span></span>

|<span data-ttu-id="9fd2c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9fd2c-113">**Element**</span></span>|<span data-ttu-id="9fd2c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9fd2c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fd2c-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="9fd2c-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="9fd2c-116">Définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié.</span><span class="sxs-lookup"><span data-stu-id="9fd2c-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9fd2c-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9fd2c-117">Text value</span></span>

<span data-ttu-id="9fd2c-118">La valeur de texte est une chaîne qui représente l’identificateur du dossier partagé pour lequel l’identificateur de dossier local doit être retournée par une demande [d’opération GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9fd2c-118">The text value is a string that represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9fd2c-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="9fd2c-119">Remarks</span></span>

<span data-ttu-id="9fd2c-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fd2c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fd2c-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9fd2c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fd2c-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9fd2c-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9fd2c-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9fd2c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9fd2c-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9fd2c-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9fd2c-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9fd2c-125">Validation File</span></span>  <br/> |<span data-ttu-id="9fd2c-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9fd2c-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9fd2c-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9fd2c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9fd2c-128">False</span><span class="sxs-lookup"><span data-stu-id="9fd2c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9fd2c-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9fd2c-129">See also</span></span>



[<span data-ttu-id="9fd2c-130">Opération GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="9fd2c-130">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="9fd2c-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9fd2c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

