---
title: GetUserPhotoResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54d43fe6-9f7b-4f84-920a-bd686c65b059
description: L’élément GetUserPhotoResponseMessage contient la réponse à une demande GetUserPhoto.
ms.openlocfilehash: a6df1204d4ac3a976694afbca008852acef6a76e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463299"
---
# <a name="getuserphotoresponsemessage"></a><span data-ttu-id="412de-103">GetUserPhotoResponseMessage</span><span class="sxs-lookup"><span data-stu-id="412de-103">GetUserPhotoResponseMessage</span></span>

<span data-ttu-id="412de-104">L’élément **GetUserPhotoResponseMessage** contient la réponse à une demande GetUserPhoto.</span><span class="sxs-lookup"><span data-stu-id="412de-104">The **GetUserPhotoResponseMessage** element contains the response to a GetUserPhoto request.</span></span> 
  
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

 <span data-ttu-id="412de-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="412de-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="412de-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="412de-106">Attributes and elements</span></span>

<span data-ttu-id="412de-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="412de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="412de-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="412de-108">Attributes</span></span>

<span data-ttu-id="412de-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="412de-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="412de-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="412de-110">Child elements</span></span>

<span data-ttu-id="412de-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [HasChanged](haschanged.md)  |  [PictureData](picturedata.md)</span><span class="sxs-lookup"><span data-stu-id="412de-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [PictureData](picturedata.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="412de-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="412de-112">Parent elements</span></span>

[<span data-ttu-id="412de-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="412de-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="412de-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="412de-114">Remarks</span></span>

<span data-ttu-id="412de-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="412de-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="412de-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="412de-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="412de-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="412de-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="412de-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="412de-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="412de-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="412de-119">Schema name</span></span>  <br/> |<span data-ttu-id="412de-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="412de-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="412de-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="412de-121">Validation file</span></span>  <br/> |<span data-ttu-id="412de-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="412de-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="412de-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="412de-123">Can be empty</span></span>  <br/> ||
   

