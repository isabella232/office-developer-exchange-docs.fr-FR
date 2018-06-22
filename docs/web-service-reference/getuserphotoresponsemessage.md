---
title: GetUserPhotoResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54d43fe6-9f7b-4f84-920a-bd686c65b059
description: L’élément GetUserPhotoResponseMessage contient la réponse à une demande de GetUserPhoto.
ms.openlocfilehash: fa817b59527f616afed84d8548e3a18e6c971e2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827696"
---
# <a name="getuserphotoresponsemessage"></a><span data-ttu-id="b4c0d-103">GetUserPhotoResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b4c0d-103">GetUserPhotoResponseMessage</span></span>

<span data-ttu-id="b4c0d-104">L’élément **GetUserPhotoResponseMessage** contient la réponse à une demande de GetUserPhoto.</span><span class="sxs-lookup"><span data-stu-id="b4c0d-104">The **GetUserPhotoResponseMessage** element contains the response to a GetUserPhoto request.</span></span> 
  
```XML
<GetUserPhotoResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <HasChanged/>
   <PictureData/>
</GetUserPhotoResponseMessage>
```

 <span data-ttu-id="b4c0d-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b4c0d-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4c0d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b4c0d-106">Attributes and elements</span></span>

<span data-ttu-id="b4c0d-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b4c0d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4c0d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b4c0d-108">Attributes</span></span>

<span data-ttu-id="b4c0d-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b4c0d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4c0d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b4c0d-110">Child elements</span></span>

<span data-ttu-id="b4c0d-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [PictureData](picturedata.md)</span><span class="sxs-lookup"><span data-stu-id="b4c0d-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [PictureData](picturedata.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b4c0d-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b4c0d-112">Parent elements</span></span>

[<span data-ttu-id="b4c0d-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b4c0d-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="b4c0d-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="b4c0d-114">Remarks</span></span>

<span data-ttu-id="b4c0d-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b4c0d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b4c0d-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4c0d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4c0d-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b4c0d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4c0d-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b4c0d-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b4c0d-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b4c0d-119">Schema name</span></span>  <br/> |<span data-ttu-id="b4c0d-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b4c0d-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b4c0d-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b4c0d-121">Validation file</span></span>  <br/> |<span data-ttu-id="b4c0d-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b4c0d-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b4c0d-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b4c0d-123">Can be empty</span></span>  <br/> ||
   

