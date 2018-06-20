---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: L’élément Position spécifie la position d’une entité extraite d’un message.
ms.openlocfilehash: 4bd8f3088891e918e13d5ef1ec8e3e5217cb3fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828853"
---
# <a name="position"></a><span data-ttu-id="3ba03-103">Position</span><span class="sxs-lookup"><span data-stu-id="3ba03-103">Position</span></span>

<span data-ttu-id="3ba03-104">L’élément **Position** spécifie la position d’une entité extraite d’un message.</span><span class="sxs-lookup"><span data-stu-id="3ba03-104">The **Position** element specifies the position of an entity extracted from a message.</span></span> 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 <span data-ttu-id="3ba03-105">**EmailPositionType**</span><span class="sxs-lookup"><span data-stu-id="3ba03-105">**EmailPositionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3ba03-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3ba03-106">Attributes and elements</span></span>

<span data-ttu-id="3ba03-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3ba03-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ba03-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3ba03-108">Attributes</span></span>

<span data-ttu-id="3ba03-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3ba03-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ba03-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3ba03-110">Child elements</span></span>

<span data-ttu-id="3ba03-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3ba03-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3ba03-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3ba03-112">Parent elements</span></span>

<span data-ttu-id="3ba03-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [Contact (TypeContact)](contact-contacttype.md) | [téléphone (PhoneEntityType)](phone-phoneentitytype.md)  |  [ TaskSuggestion](tasksuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="3ba03-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [Contact (ContactType)](contact-contacttype.md) | [Phone (PhoneEntityType)](phone-phoneentitytype.md) | [TaskSuggestion](tasksuggestion.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3ba03-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3ba03-114">Text value</span></span>

<span data-ttu-id="3ba03-115">La valeur de texte de l’élément **Position** est l’emplacement où une entité extraite à l’origine dans le message source.</span><span class="sxs-lookup"><span data-stu-id="3ba03-115">The text value of the **Position** element is the location where an extracted entity originated in the source message.</span></span> <span data-ttu-id="3ba03-116">Les valeurs de texte de l’élément **Position** sont :</span><span class="sxs-lookup"><span data-stu-id="3ba03-116">The text values for the **Position** element are:</span></span> 
  
- <span data-ttu-id="3ba03-117">**LatestReply** - l’entité extraite provient de la réponse au message le plus récent.</span><span class="sxs-lookup"><span data-stu-id="3ba03-117">**LatestReply** - the extracted entity originates from the latest reply to the message.</span></span> 
    
- <span data-ttu-id="3ba03-118">**Autres** - l’entité extraite provient d’une partie du message non définie.</span><span class="sxs-lookup"><span data-stu-id="3ba03-118">**Other** - the extracted entity originates from an undefined part of the message.</span></span> 
    
- <span data-ttu-id="3ba03-119">**Objet** : l’entité extraite provient de l’objet du message.</span><span class="sxs-lookup"><span data-stu-id="3ba03-119">**Subject** - the extracted entity originates from the message subject.</span></span> 
    
- <span data-ttu-id="3ba03-120">**Signature** - l’entité extraite provient de la signature du message.</span><span class="sxs-lookup"><span data-stu-id="3ba03-120">**Signature** - the extracted entity originates from the message signature.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="3ba03-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="3ba03-121">Remarks</span></span>

<span data-ttu-id="3ba03-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3ba03-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3ba03-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ba03-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ba03-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3ba03-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ba03-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3ba03-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3ba03-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3ba03-126">Schema name</span></span>  <br/> |<span data-ttu-id="3ba03-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3ba03-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="3ba03-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3ba03-128">Validation file</span></span>  <br/> |<span data-ttu-id="3ba03-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3ba03-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3ba03-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3ba03-130">Can be empty</span></span>  <br/> ||
   

