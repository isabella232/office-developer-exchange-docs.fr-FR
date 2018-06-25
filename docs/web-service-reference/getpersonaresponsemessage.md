---
title: GetPersonaResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a5bf44c6-c46b-442d-98d4-8b49fdf14b30
description: La GetPersonaResponseMessage contient les données de réponse résultant d’une demande GetPersona.
ms.openlocfilehash: 7d38daac9c7c3a74ba9d9670c2bd16dcf2cd47e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756717"
---
# <a name="getpersonaresponsemessage"></a><span data-ttu-id="79db9-103">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="79db9-103">GetPersonaResponseMessage</span></span>

<span data-ttu-id="79db9-104">La **GetPersonaResponseMessage** contient les données de réponse résultant d’une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="79db9-104">The **GetPersonaResponseMessage** contains the response data resulting from a **GetPersona** request.</span></span> 
  
```XML
<GetPersonaResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Persona/>
</GetPersonaResponseMessage>
```

 <span data-ttu-id="79db9-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="79db9-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79db9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="79db9-106">Attributes and elements</span></span>

<span data-ttu-id="79db9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="79db9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79db9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="79db9-108">Attributes</span></span>

<span data-ttu-id="79db9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79db9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79db9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="79db9-110">Child elements</span></span>

<span data-ttu-id="79db9-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [personnage](persona.md)</span><span class="sxs-lookup"><span data-stu-id="79db9-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Persona](persona.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79db9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="79db9-112">Parent elements</span></span>

[<span data-ttu-id="79db9-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="79db9-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="79db9-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="79db9-114">Remarks</span></span>

<span data-ttu-id="79db9-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="79db9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="79db9-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="79db9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79db9-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="79db9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79db9-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="79db9-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="79db9-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="79db9-119">Schema name</span></span>  <br/> |<span data-ttu-id="79db9-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="79db9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="79db9-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="79db9-121">Validation file</span></span>  <br/> |<span data-ttu-id="79db9-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="79db9-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="79db9-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="79db9-123">Can be empty</span></span>  <br/> ||
   

