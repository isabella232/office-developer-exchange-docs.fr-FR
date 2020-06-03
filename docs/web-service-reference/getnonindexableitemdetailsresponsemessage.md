---
title: GetNonIndexableItemDetailsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00566965-6cbd-4f31-9fa9-85b3e5559c0c
description: L’élément GetNonIndexableItemDetailsResponseMessage spécifie le message de réponse pour une demande GetNonIndexableItemDetails.
ms.openlocfilehash: 4cf6b422cc29b20b09d05ea45628fa7133b437b2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456520"
---
# <a name="getnonindexableitemdetailsresponsemessage"></a><span data-ttu-id="de4e9-103">GetNonIndexableItemDetailsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="de4e9-103">GetNonIndexableItemDetailsResponseMessage</span></span>

<span data-ttu-id="de4e9-104">L’élément **GetNonIndexableItemDetailsResponseMessage** spécifie le message de réponse pour une demande **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="de4e9-104">The **GetNonIndexableItemDetailsResponseMessage** element specifies the response message for a **GetNonIndexableItemDetails** request.</span></span> 
  
```XML
<GetNonIndexableItemDetailsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <NonIndexableItemDetailsResult/>
</GetNonIndexableItemDetailsResponseMessage>
```

 <span data-ttu-id="de4e9-105">**GetNonIndexableItemDetailsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="de4e9-105">**GetNonIndexableItemDetailsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de4e9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="de4e9-106">Attributes and elements</span></span>

<span data-ttu-id="de4e9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="de4e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de4e9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="de4e9-108">Attributes</span></span>

<span data-ttu-id="de4e9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="de4e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de4e9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="de4e9-110">Child elements</span></span>

<span data-ttu-id="de4e9-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span><span class="sxs-lookup"><span data-stu-id="de4e9-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="de4e9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="de4e9-112">Parent elements</span></span>

[<span data-ttu-id="de4e9-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="de4e9-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="de4e9-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="de4e9-114">Remarks</span></span>

<span data-ttu-id="de4e9-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="de4e9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="de4e9-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="de4e9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de4e9-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="de4e9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de4e9-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="de4e9-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="de4e9-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="de4e9-119">Schema name</span></span>  <br/> |<span data-ttu-id="de4e9-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="de4e9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="de4e9-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="de4e9-121">Validation file</span></span>  <br/> |<span data-ttu-id="de4e9-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="de4e9-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="de4e9-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="de4e9-123">Can be empty</span></span>  <br/> |<span data-ttu-id="de4e9-124">false</span><span class="sxs-lookup"><span data-stu-id="de4e9-124">false</span></span>  <br/> |
   

