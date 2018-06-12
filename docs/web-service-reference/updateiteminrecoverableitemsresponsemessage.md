---
title: UpdateItemInRecoverableItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96259756-322e-4c24-ac76-0cd9c32e0d6d
description: L’élément UpdateItemInRecoverableItemsResponseMessage spécifie la réponse à une demande de UpdateItemInRecoverableItems.
ms.openlocfilehash: 598d91a4fbd4d241b75aea4c155caca68f120b3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838892"
---
# <a name="updateiteminrecoverableitemsresponsemessage"></a><span data-ttu-id="bb1bf-103">UpdateItemInRecoverableItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bb1bf-103">UpdateItemInRecoverableItemsResponseMessage</span></span>

<span data-ttu-id="bb1bf-104">L’élément **UpdateItemInRecoverableItemsResponseMessage** spécifie la réponse à une demande de **UpdateItemInRecoverableItems** .</span><span class="sxs-lookup"><span data-stu-id="bb1bf-104">The **UpdateItemInRecoverableItemsResponseMessage** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
```XML
<UpdateItemInRecoverableItemsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKet/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponseMessage>
```

 <span data-ttu-id="bb1bf-105">**UpdateItemInRecoverableItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bb1bf-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb1bf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bb1bf-106">Attributes and elements</span></span>

<span data-ttu-id="bb1bf-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bb1bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb1bf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bb1bf-108">Attributes</span></span>

<span data-ttu-id="bb1bf-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bb1bf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb1bf-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bb1bf-110">Child elements</span></span>

<span data-ttu-id="bb1bf-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [éléments](items.md) | [pièces jointes](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span><span class="sxs-lookup"><span data-stu-id="bb1bf-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bb1bf-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bb1bf-112">Parent elements</span></span>

<span data-ttu-id="bb1bf-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bb1bf-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bb1bf-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="bb1bf-114">Remarks</span></span>

<span data-ttu-id="bb1bf-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bb1bf-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bb1bf-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb1bf-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb1bf-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bb1bf-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb1bf-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bb1bf-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="bb1bf-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bb1bf-119">Schema name</span></span>  <br/> |<span data-ttu-id="bb1bf-120">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="bb1bf-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="bb1bf-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bb1bf-121">Validation file</span></span>  <br/> |<span data-ttu-id="bb1bf-122">Message.xsd</span><span class="sxs-lookup"><span data-stu-id="bb1bf-122">Message.xsd</span></span>  <br/> |
|<span data-ttu-id="bb1bf-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bb1bf-123">Can be empty</span></span>  <br/> |<span data-ttu-id="bb1bf-124">false</span><span class="sxs-lookup"><span data-stu-id="bb1bf-124">false</span></span>  <br/> |
   
