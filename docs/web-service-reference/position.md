---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: L’élément position spécifie la position d’une entité extraite d’un message.
ms.openlocfilehash: 9acd965c3e0c29f3fa91df338c0671749192b38b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465421"
---
# <a name="position"></a><span data-ttu-id="8ebf4-103">Position</span><span class="sxs-lookup"><span data-stu-id="8ebf4-103">Position</span></span>

<span data-ttu-id="8ebf4-104">L’élément **position** spécifie la position d’une entité extraite d’un message.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-104">The **Position** element specifies the position of an entity extracted from a message.</span></span> 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 <span data-ttu-id="8ebf4-105">**EmailPositionType**</span><span class="sxs-lookup"><span data-stu-id="8ebf4-105">**EmailPositionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ebf4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8ebf4-106">Attributes and elements</span></span>

<span data-ttu-id="8ebf4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ebf4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8ebf4-108">Attributes</span></span>

<span data-ttu-id="8ebf4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ebf4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8ebf4-110">Child elements</span></span>

<span data-ttu-id="8ebf4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ebf4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8ebf4-112">Parent elements</span></span>

<span data-ttu-id="8ebf4-113">[UrlEntity](urlentity.md)  |  [AddressEntity](addressentity.md)  |  [EmailAddressEntity](emailaddressentity.md)  |  [MeetingSuggestion](meetingsuggestion.md)  |  [Contact (ContactType)](contact-contacttype.md)  |  [Téléphone (PhoneEntityType)](phone-phoneentitytype.md)  |  [TaskSuggestion](tasksuggestion.md)</span><span class="sxs-lookup"><span data-stu-id="8ebf4-113">[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [Contact (ContactType)](contact-contacttype.md) | [Phone (PhoneEntityType)](phone-phoneentitytype.md) | [TaskSuggestion](tasksuggestion.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="8ebf4-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="8ebf4-114">Text value</span></span>

<span data-ttu-id="8ebf4-115">La valeur de texte de l’élément **position** est l’emplacement où provient une entité extraite dans le message source.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-115">The text value of the **Position** element is the location where an extracted entity originated in the source message.</span></span> <span data-ttu-id="8ebf4-116">Les valeurs de texte de l’élément **position** sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="8ebf4-116">The text values for the **Position** element are:</span></span> 
  
- <span data-ttu-id="8ebf4-117">**LatestReply** -l’entité extraite provient de la dernière réponse du message.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-117">**LatestReply** - the extracted entity originates from the latest reply to the message.</span></span> 
    
- <span data-ttu-id="8ebf4-118">**Other** : l’entité extraite provient d’une partie non définie du message.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-118">**Other** - the extracted entity originates from an undefined part of the message.</span></span> 
    
- <span data-ttu-id="8ebf4-119">**Subject** : l’entité extraite provient de l’objet du message.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-119">**Subject** - the extracted entity originates from the message subject.</span></span> 
    
- <span data-ttu-id="8ebf4-120">**Signature** : l’entité extraite provient de la signature du message.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-120">**Signature** - the extracted entity originates from the message signature.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="8ebf4-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="8ebf4-121">Remarks</span></span>

<span data-ttu-id="8ebf4-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8ebf4-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ebf4-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ebf4-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8ebf4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ebf4-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8ebf4-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8ebf4-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8ebf4-126">Schema name</span></span>  <br/> |<span data-ttu-id="8ebf4-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8ebf4-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="8ebf4-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8ebf4-128">Validation file</span></span>  <br/> |<span data-ttu-id="8ebf4-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8ebf4-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8ebf4-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8ebf4-130">Can be empty</span></span>  <br/> ||
   

