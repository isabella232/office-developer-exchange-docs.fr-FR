---
title: GetUserRetentionPolicyTagsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9991d6e0-8c31-4e73-8af3-da4298474b66
description: L’élément GetUserRetentionPolicyTagsResponseMessage spécifie le message de réponse pour une demande GetUserRetentionPolicyTags.
ms.openlocfilehash: e65266e72010f42a2052bbb8cfab21ea4059f92b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461806"
---
# <a name="getuserretentionpolicytagsresponsemessage"></a><span data-ttu-id="f40c3-103">GetUserRetentionPolicyTagsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f40c3-103">GetUserRetentionPolicyTagsResponseMessage</span></span>

<span data-ttu-id="f40c3-104">L’élément **GetUserRetentionPolicyTagsResponseMessage** spécifie le message de réponse pour une demande **GetUserRetentionPolicyTags** .</span><span class="sxs-lookup"><span data-stu-id="f40c3-104">The **GetUserRetentionPolicyTagsResponseMessage** element specifies the response message for a **GetUserRetentionPolicyTags** request.</span></span> 
  
```XML
<GetUserRetentionPolicyTagsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RetentionPolicyTags/>
</GetUserRetentionPolicyTagsResponseMessage>
```

 <span data-ttu-id="f40c3-105">**GetUserRetentionPolicyTagsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f40c3-105">**GetUserRetentionPolicyTagsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f40c3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f40c3-106">Attributes and elements</span></span>

<span data-ttu-id="f40c3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f40c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f40c3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f40c3-108">Attributes</span></span>

<span data-ttu-id="f40c3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f40c3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f40c3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f40c3-110">Child elements</span></span>

<span data-ttu-id="f40c3-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [RetentionPolicyTags](retentionpolicytags.md)</span><span class="sxs-lookup"><span data-stu-id="f40c3-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f40c3-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f40c3-112">Parent elements</span></span>

[<span data-ttu-id="f40c3-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f40c3-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="f40c3-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="f40c3-114">Remarks</span></span>

<span data-ttu-id="f40c3-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f40c3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f40c3-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f40c3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f40c3-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f40c3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f40c3-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f40c3-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f40c3-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f40c3-119">Schema name</span></span>  <br/> |<span data-ttu-id="f40c3-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f40c3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f40c3-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f40c3-121">Validation file</span></span>  <br/> |<span data-ttu-id="f40c3-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f40c3-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f40c3-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f40c3-123">Can be empty</span></span>  <br/> |<span data-ttu-id="f40c3-124">false</span><span class="sxs-lookup"><span data-stu-id="f40c3-124">false</span></span>  <br/> |
   

