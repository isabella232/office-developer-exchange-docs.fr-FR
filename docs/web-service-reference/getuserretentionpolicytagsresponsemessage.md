---
title: GetUserRetentionPolicyTagsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9991d6e0-8c31-4e73-8af3-da4298474b66
description: L’élément GetUserRetentionPolicyTagsResponseMessage Spécifie le message de réponse pour une demande GetUserRetentionPolicyTags.
ms.openlocfilehash: db73cb7f1922d845c9565753ff8d4917b82b1259
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19827701"
---
# <a name="getuserretentionpolicytagsresponsemessage"></a><span data-ttu-id="6ff5c-103">GetUserRetentionPolicyTagsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6ff5c-103">GetUserRetentionPolicyTagsResponseMessage</span></span>

<span data-ttu-id="6ff5c-104">L’élément **GetUserRetentionPolicyTagsResponseMessage** Spécifie le message de réponse pour une demande **GetUserRetentionPolicyTags** .</span><span class="sxs-lookup"><span data-stu-id="6ff5c-104">The **GetUserRetentionPolicyTagsResponseMessage** element specifies the response message for a **GetUserRetentionPolicyTags** request.</span></span> 
  
```XML
<GetUserRetentionPolicyTagsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RetentionPolicyTags/>
</GetUserRetentionPolicyTagsResponseMessage>
```

 <span data-ttu-id="6ff5c-105">**GetUserRetentionPolicyTagsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6ff5c-105">**GetUserRetentionPolicyTagsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ff5c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6ff5c-106">Attributes and elements</span></span>

<span data-ttu-id="6ff5c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6ff5c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ff5c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6ff5c-108">Attributes</span></span>

<span data-ttu-id="6ff5c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6ff5c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ff5c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6ff5c-110">Child elements</span></span>

<span data-ttu-id="6ff5c-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)</span><span class="sxs-lookup"><span data-stu-id="6ff5c-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6ff5c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6ff5c-112">Parent elements</span></span>

[<span data-ttu-id="6ff5c-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6ff5c-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="6ff5c-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="6ff5c-114">Remarks</span></span>

<span data-ttu-id="6ff5c-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6ff5c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6ff5c-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ff5c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ff5c-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6ff5c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ff5c-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6ff5c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6ff5c-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6ff5c-119">Schema name</span></span>  <br/> |<span data-ttu-id="6ff5c-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6ff5c-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6ff5c-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6ff5c-121">Validation file</span></span>  <br/> |<span data-ttu-id="6ff5c-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6ff5c-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6ff5c-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6ff5c-123">Can be empty</span></span>  <br/> |<span data-ttu-id="6ff5c-124">false</span><span class="sxs-lookup"><span data-stu-id="6ff5c-124">false</span></span>  <br/> |
   

